# FizzBuzz
//
//  ViewController.swift
//  FizzBuzz
//
//  Created by Derek Rodriguez Martinez on 10/30/19.
//  Copyright © 2019 Derek Rodriguez Martinez. All rights reserved.
//

import UIKit
import Foundation

class ViewController: UIViewController {

    var numberIn = 0;
    
    @IBAction func textInputted(_ sender: Any) {
        numberIn = Int(textField.text!)!
    }
    
    @IBOutlet var textField: UITextField!
    
    @IBAction func userConfirm(_ sender: Any) {
        for i in 1...numberIn {
            if i % 3 == 0 {
                if i % 5 == 0 {
                    if i % 7 == 0 {
                        print ("Fizz-Buzz-Bang")
                    }
                    else {
                        print ("Fizz-Buzz")
                    }
                }
                else {
                    print ("Fizz")
                }
            }
            else if i % 5 == 0 {
                print ("Buzz")
            }
            else if i % 7 == 0 {
                print ("Bang")
            }
            else {
                print (i)
            }
        }
