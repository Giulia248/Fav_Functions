# Fav_Functions
My most used functions 

[Button + Label](#Button-and-labels)  
[Custom Color](#custom-colour)  
[url image](#image-by-url)  
[change view](#change-view) 
[change view2](#change-view2)



[GitHub readMe Functions](#GitHub-readMe-Functions)  

## Button and Labels

```
                  
                  Button {
                    
                    //actions
                                         
            }label :{
    Text("label").padding().foregroundColor(.black).font(.system(size: 30)).overlay(RoundedRectangle(cornerRadius:50).stroke(Color.black,   lineWidth: 5))  
                
            }.offset(x: 0, y: 300)
            //-------------------------
            //button with icon/image
            Button(action: {
    // Do something...
    }, label: {
        Image("download")
    })
        //-------------------------
        Text("label").font(.system(size: 20)).frame(width: 300, height: 300, alignment: .center).padding().lineLimit(100)
```
[go up](#Fav_Functions)  

## custom colour

```

    struct CustomColor {
      static let myColor = Color("mycolor")
      // Add more here...
    }
    .foregroundColor(CustomColor.myColor)
   
```
[go up](#Fav_Functions)  

## image by url

```

    AsyncImage(url: URL(string: "url"))

```
[go up](#Fav_Functions)  

## change view

```

                NavigationView{
            ZStack{
                Image("background").scaledToFit().ignoresSafeArea()
                VStack{
                    Text(" ")
                    Spacer().frame( height: 200)
                    NavigationLink(destination: view()) {
                        
                        Label( "", systemImage: "").font(.system(size: 20))
                      
                    }.frame(width: 200, height: 200, alignment: .bottom)
                }
                 
                }
        }

```

## change view2

```

         TabView {
            ZStack {
                Image("a").scaledToFill().ignoresSafeArea()
                
                
            }
            Insects()
                       .tabItem {
                           Label("Seleziona insetto", systemImage: "ant")
                               .navigationTitle("")
                               
                               
                       }

        }.onAppear() {
            UITabBar.appearance().backgroundColor = .gray
            .withAlphaComponent(0.8)
            
        
```

[go up](#Fav_Functions)  


# GitHub readMe Functions

## Links

" [title].(link)  "

## Backtick code frame
` ` ` ` ` `


