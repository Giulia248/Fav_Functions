# Fav_Functions
My most used functions 

[Bottoni](#Button)  
[Custom Color](#custom-colour)  
[url image](#image-by-url)  
[change view](#change-view)  

## Button

'
                  
                  Button {
                
                //actions
                     
                 
                 
            }label :{
    Text("label").padding().foregroundColor(CustomColor.verde).font(.system(size: 30)).overlay(RoundedRectangle(cornerRadius:50).stroke(Color.black,   lineWidth: 5))  
                
            }.offset(x: 0, y: 300)


'

## custom colour

'

    struct CustomColor {
      static let myColor = Color("mycolor")
      // Add more here...
    }
    .foregroundColor(CustomColor.myColor)
   
'

## image by url

'

    AsyncImage(url: URL(string: "url"))

'

## change view

'

        NavigationView{
            ZStack{
                Image("background").resizable().frame(width: 800, height: 1000)
                 NavigationLink(destination: ContentView2()) {
                   Text("button").padding().foregroundColor(CustomColor.verde).font(.system(size: 30)).overlay(RoundedRectangle(cornerRadius:50).stroke(Color.black, lineWidth: 5))              
                    }  
                } 
        }

'

