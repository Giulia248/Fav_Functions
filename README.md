# Fav_Functions
My most used functions 

[Button + Label](#Button-and-labels)  
[Custom Color](#custom-colour)  
[url image](#image-by-url)  
[change view](#change-view) 
[change view2](#change-view2)  

## Button and Labels

'
                  
                  Button {
                    
                    //actions
                                         
            }label :{
    Text("label").padding().foregroundColor(.black).font(.system(size: 30)).overlay(RoundedRectangle(cornerRadius:50).stroke(Color.black,   lineWidth: 5))  
                
            }.offset(x: 0, y: 300)
    //-------------------------
    Text("label").padding().foregroundColor(.black).font(.system(size: 30)).offset(x: 0, y: 0)

'
[go up](#Fav_Functions)  

## custom colour

'

    struct CustomColor {
      static let myColor = Color("mycolor")
      // Add more here...
    }
    .foregroundColor(CustomColor.myColor)
   
'
[go up](#Fav_Functions)  

## image by url

'

    AsyncImage(url: URL(string: "url"))

'
[go up](#Fav_Functions)  

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

#change view2
'
        TabView {
                  View1()
                       .tabItem {
                           Label("label", systemImage: "qrcode.viewfinder").foregroundColor(.black)
                               .navigationTitle("View1")
                       }

                  View2()
                       .tabItem {
                           Label("label", systemImage: "qrcode.viewfinder").foregroundColor(.black)
                               .navigationTitle("View2")
                       }

        }
'

