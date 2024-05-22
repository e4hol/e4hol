 Mobile Device class
class MobileDevice {
    public MobileDevice() {
    }

    public void turnOn() {
        System.out.println("Mobile Device is turning on.");
    }

    public void turnOff() {
        System.out.println("Mobile Device is turning off.");
    }
}

// Mobile Phone class as a subclass
class MobilePhone extends MobileDevice {
    public MobilePhone() {
        super();
    }

    @Override
    public void turnOn() {
        System.out.println("Mobile Phone is turning on.");
    }

    @Override
    public void turnOff() {
        System.out.println("Mobile Phone is turning off.");
    }
}

// Laptop class as a subclass
class Laptop extends MobileDevice {
    public Laptop() {
        super();
    }

    @Override
    public void turnOn() {
        System.out.println("Laptop is turning on.");
    }

    @Override
    public void turnOff() {
        System.out.println("Laptop is turning off.");
    }
}

// Main class to create objects and invoke methods
public class Main {
    public static void main(String[] args) {
        MobileDevice mobileDevice = new MobileDevice();
        MobilePhone mobilePhone = new MobilePhone();
        Laptop laptop = new Laptop();

        mobileDevice.turnOn();
        mobileDevice.turnOff();

        mobilePhone.turnOn();
        mobilePhone.turnOff();

        laptop.turnOn();
        laptop.turnOff();
    }
}
