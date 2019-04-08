# Overview

Requirements regarding the application.
Explanation of terms:
* An item is an article that can be bought on the Kinderkleidermarket
* A data storage is a possibility to store item data (data base, csv file, ...)
* A customer is someone who wants to buy something on the Kinderkleidermarket
* A seller is someone who wants to sell something on the Kinderkleidermarket
* Booking in and out describes actions to change items state within the data storage

## Hardware
* Communication between a barcode scanner and a device
    * Scanner: dedicated hardware? mobile phone? webcam?
        * Dedicated hardware: which interface? emulated keyboard or USB?
    * Device: mobile phone (Android)? PC (Windows)?
* Possibility to support more than one device at once?

## Software

Must be simple and usable by everyone

* Type 

* Cashier-Mode (Checkout, "Kassenmodus")
    * Items can be booked out (change item state within data storage)
    * Generate list for buyer with items bought
    * Possibility to book items in again ("I don't want to buy it after all!")
    * Button: "New Customer"
    * Button: "Reset"
    * Possibility to add items manually (without barcode in case it cannot be read)
    
<!-- * The scanner must be operated in two different modes: -->
<!--   * A: -->

* Data table entries
    * Seller Name
    * Seller ID
    * Price in €
    * Item name (optional)
    * Timestamp booked in
    * Timestamp booked out
    * Color (optional)
    * Item State
        * Booked in ("At sale")
        * Booked out ("Sold")
        * Unknown ("Lost") <<- ?
        
* Printer interface
    * PyLaTeX support for PDF generation?
    * Receipt?
    * Would need a GUI button ("Print xxx")
    
* Overview for seller when getting items/money back
    * Which items were sold and how much money will be returned (excluding fees)
    * Which items were not sold, 
    
* Global overview
    * How many items sold/not sold
    * Display for revenue

## Environment
* Backup the data storage on an external memory

## Problems
* How to get new items into the data structure

## To check
* What barcode is available on the item labels

## Nice to have
* Touchable GUI
* Café and cake merged into this (with barcode)

## Use-cases to check
* Customer at the cashier, process to scan items started
-> Process is interrupted, another customer is cashed first
* What if price on label and price in database do not match (correction mode?)
