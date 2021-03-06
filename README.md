# Weekend Challenge 2#: Take away challenge [![Build Status](https://travis-ci.org/thatdania/takeaway-challenge.svg?branch=master)](https://travis-ci.org/thatdania/takeaway-challenge)

```
                            _________
              r==           |       |
           _  //            |  M.A. |   ))))
          |_)//(''''':      |       |
            //  \_____:_____.-------D     )))))
           //   | ===  |   /        \
       .:'//.   \ \=|   \ /  .:'':./    )))))
      :' // ':   \ \ ''..'--:'-.. ':
      '. '' .'    \:.....:--'.-'' .'
       ':..:'                ':..:'

 ```


## How to Use 🥘🥗

![](images/Screen%20Shot%202017-11-06%20at%2009.48.39.png)


### Design Approach

I had several design draft on how my code would look like before I attempted it. A lot of the experimentation in pry took time to understand what the user needed to see in the format of Ruby. It took be a while to think of this project like Deliveroo, and thus, have a printed menu with options that could be actions for the program.

### Explanation

As we go through the screen shot, we first see a printed menu with number options. You then can click the options to see what the program develops into.It takes the orders if you click 1-4, it prints out the whole order if you click 5, it then tells you the total if you click 7 and then it tells you to go to payment. The payment (or check out method) has three situations where it either gets money that is not equal or equal to the amount. A computer wouldn't take more than the amount stated neither would a customer give more than the amount staed if it were digital. Hence, I changed my initial approach of allowing the computer to give change to just having a value not equal to something. 

### Unit Test

I believe most unit tests are design to check every feature in the program I have created so far. This is especially with the options the user can choose. I either drew out what I was going to test or featured tested it in pry. You can check in the spec folders.

### Future Improvements

If I had more time, I would work out a method on how to remove a chosen order from a list and dive deeper into twilio as that was our extra challenge for the day.Obviously, where the checkout method ends with you will receive a confirmation, the twilio aspect of this project will continue on from there.


## Domain Model

| Objects            | Messages      | Output            |
| ------------------ |:-------------:| -----------------:|
| list(dishes,prices)| see           | See A menu?       |
| dishes             | select        | Select dishes     |
| total, sum         | compare/check | Match 2 prices    |
| receive text       | receive       | Text confirmation |


## Supported Documents
- https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet (Markdown for Domain Model)
- https://ruby-doc.org/core-2.4.2/Hash.html (To understand hashes)
- https://stackoverflow.com/questions/18984390/accessing-array-of-hashes (Understand the array of hashes)
- https://relishapp.com/rspec/rspec-expectations/v/3-7/docs/built-in-matchers/include-matcher
- https://www.twilio.com/ (As A Trial)
