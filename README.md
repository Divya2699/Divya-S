Here's a simple example of Java code that models a Computer Hardware System using object-oriented programming concepts. This code defines classes for basic hardware components: CPU, RAM, HardDrive, and a ComputerSystem that brings them together.

// CPU class
class CPU {
    String model;
    double speedGHz;

    public CPU(String model, double speedGHz) {
        this.model = model;
        this.speedGHz = speedGHz;
    }

    public void displayInfo() {
        System.out.println("CPU Model: " + model + ", Speed: " + speedGHz + " GHz");
    }
}

// RAM class
class RAM {
    int sizeGB;

    public RAM(int sizeGB) {
        this.sizeGB = sizeGB;
    }

    public void displayInfo() {
        System.out.println("RAM Size: " + sizeGB + " GB");
    }
}

// HardDrive class
class HardDrive {
    int capacityGB;
    String type;

    public HardDrive(int capacityGB, String type) {
        this.capacityGB = capacityGB;
        this.type = type;
    }

    public void displayInfo() {
        System.out.println("Hard Drive: " + capacityGB + " GB " + type);
    }
}

// ComputerSystem class
class ComputerSystem {
    CPU cpu;
    RAM ram;
    HardDrive hardDrive;

    public ComputerSystem(CPU cpu, RAM ram, HardDrive hardDrive) {
        this.cpu = cpu;
        this.ram = ram;
        this.hardDrive = hardDrive;
    }

    public void displaySystemInfo() {
        System.out.println("Computer System Info:");
        cpu.displayInfo();
        ram.displayInfo();
        hardDrive.displayInfo();
    }
}

// Main class to run the program
public class Main {
    public static void main(String[] args) {
        CPU cpu = new CPU("Intel i7", 3.5);
        RAM ram = new RAM(16);
        HardDrive hd = new HardDrive(512, "SSD");

        ComputerSystem system = new ComputerSystem(cpu, ram, hd);
        system.displaySystemInfo();
    }
}

Output:

Computer System Info:
CPU Model: Intel i7, Speed: 3.5 GHz
RAM Size: 16 GB
Hard Drive: 512 GB SSD

Let me know if you want to include more components (e.g., GPU, Motherboard) or add user input.

GPU# Divya-S
Project 
Computer Hardware system 