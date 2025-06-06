# verify-kaspa-address
Simple one click tool for iPhone users with the action button to verify whether a Kaspa address has ever been used before 

download the tool https://www.icloud.com/shortcuts/891e64c39e6b430daa92340e3dadc32f

How to build: 

1. If [clipboard] does not have any value, [stop this shortcut]. 
       Otherwise 
          If [clipboard] does not contain [kaspa:], [stop this shortcut] 

• What these actions do is prevent the shortcut from running if there is no text saved to the clipboard, as well as if it cannot find a kaspa address. Anything else copied to the clipboard the shortcut will not run. 

This shortcut utilizes the Kaspa API  https://api.kaspa.org/addresses/transactions-count (link here is missing a Kaspa address. Read further down on where to put it)

2. [Text] :  https://api.kaspa.org/addresses/[clipboard]/transactions-count
3. Copy the above url, replace [clipboard] with the clipboard variable as seen in the screenshot. Make sure there are no spaces or extra characters. Everything is case sensitive. Now when you copy a $kas address it will auto paste it and generate the full link
4.  [Get contents of URL] - don’t change any settings. Make sure it says GET, no extra headers.
5. Get [Dictionary Value] for [total] in [Contents of URL] 
6. [Get numbers from input] > Get numbers from [dictionary value] 
   If [Numbers] is [0] 
    Show notification [“This          Kaspa Address Has Never Been Used Before ✅”]
   Otherwise 
     Show notification [“This Kaspa Address Has Been Used [dictionary value] Times ❌”]

End

To program this shortcut to run with the press of the action button go to device settings > action button > scroll until you see shortcut > choose this shortcut 

If you do not have an action button you can run this using a widget. Add the widget where ever you’d like and search for shortcuts and find the one you just made. 

Remember, this shortcut will only run when a kaspa address is copied to the clipboard

For troubleshooting or tips you can find me on twitter at @brt2412

Support my work: kaspa:qqvmhcyp2cnh0urd8pje6mxqlckpmlfe8ltukxaqrtnd4h7t600rx4lnyuwln

![IMG_1832](https://github.com/user-attachments/assets/c568919f-b9df-443b-9e4b-81f4ea485fcb)
![IMG_1833](https://github.com/user-attachments/assets/ca9a86aa-8604-48d3-9d4a-7b6e8361b78a)
![IMG_1834](https://github.com/user-attachments/assets/6cc8bf93-a54a-4143-a146-eec8389c29a2)
![IMG_1835](https://github.com/user-attachments/assets/1b6520b8-adeb-4de6-b22b-da9f2e1851fc)
![IMG_1836](https://github.com/user-attachments/assets/a82c9014-75bf-4f98-8dff-0a5824aa00b6)
