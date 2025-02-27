/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 * Click nbfs://nbhost/SystemFileSystem/Templates/Classes/Main.java to edit this template
 */

package lab1;

import java.util.ArrayList;
import java.util.List;

/**
 *
 * @author Seby
 */
public class Lab1 {

    /**
     * @param args the command line arguments
     */
    
    static class FelMancare {
        private String name;
        private double price;
        private String description;
       
        public FelMancare(String name, double price, String description) {
            this.name = name;
            this.price = price;
            this.description = description;
        }
        
        public String getName() {
            return name;
        }
        
        public void setName(String name) {
            this.name = name;
        }

        public double getPrice() {
            return price;
        }
        
        public void setPrice(double price) {
            this.price = price;
        }

    }
    
    static abstract class Restaurant {
        protected String name;
        protected String headChef;
        protected List<FelMancare> menu;
        
        public Restaurant(String name, String headChef) {
            this.name = name;
            this.headChef = headChef;
            this.menu = new ArrayList<>();
        }

        public void addDishToMenu(FelMancare item) {
            menu.add(item);
        }
    }
    
    static class VegetarianRestaurant extends Restaurant {
        private double reducere = 0.1;
        private double taxa_livrare = 20.0; 
        
        public VegetarianRestaurant(String name, String headChef) {
            super(name, headChef);
        } 
    }
        
    static class NonVegetarianRestaurant extends Restaurant {
        private double reducere = 0.15;
        private double taxa_livrare = 10.0; 
        
        public NonVegetarianRestaurant(String name, String headChef) {
            super(name, headChef);
        }
    }
    
    public static void main(String[] args) {
        // TODO code application logic here
        // restaurante veg
        VegetarianRestaurant veg1 = new VegetarianRestaurant("Green Life", "Ana Dorohoi");
        veg1.addDishToMenu(new FelMancare("Salată", 25.0, "seminte, avocado, castraveti"));
        veg1.addDishToMenu(new FelMancare("Burger Veggie", 30.0, "Chiftea bio, sos de morcov"));
        VegetarianRestaurant veg2 = new VegetarianRestaurant("Green Food", "Andrei Popescu");
        veg2.addDishToMenu(new FelMancare("Supa de legume", 20.0, "ciuperci, morcovi, seminte"));
        veg2.addDishToMenu(new FelMancare("Menu Falafel", 28.0, "Falafel, hummus, legume"));
        
        // restaurante neveg
        NonVegetarianRestaurant neveg1 = new NonVegetarianRestaurant("Meat Life", "Alina Mihai");
        neveg1.addDishToMenu(new FelMancare("Salată", 25.0, "seminte, avocado, castraveti"));
        neveg1.addDishToMenu(new FelMancare("Burger V10", 30.0, "Chiftea, vita, maioneza, branza"));
        NonVegetarianRestaurant neveg2 = new NonVegetarianRestaurant("Meat Food", "George Simion");
        neveg2.addDishToMenu(new FelMancare("Piept de pui", 20.0, "piept pui, ciuperci"));
        neveg2.addDishToMenu(new FelMancare("Menu Shaorma", 28.0, "carne, ketchup, cartofi"));
        
    }
}

