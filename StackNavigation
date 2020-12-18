import * as React from 'react';
import { Text, View, StyleSheet,ScrollView ,TouchableOpacity} from 'react-native';
import Constants from 'expo-constants';
import { Card,DataTable } from 'react-native-paper';
import { NavigationContainer } from '@react-navigation/native';
import { createStackNavigator } from '@react-navigation/stack';
import 'react-native-gesture-handler';
import BTN from "./components/CustomButton"
import { Ionicons, FontAwesome } from '@expo/vector-icons';
import { ListItem, Icon } from 'react-native-elements'

class ProductDetails extends React.Component{
  render(){
    const products=[this.props.route.params]
    return (
      <ScrollView style={{backgroundColor:"white",flex:1}}>
     <View style={{ backgroundColor:"orange",width:"33%",alignSelf:"center",marginTop:3}}><Text style={{fontSize:18,fontFamily:"Times New Roman",textAlign:"center",color:"white"}}>{this.props.route.params.name}</Text></View>
     <View><Text style={{marginLeft:8,marginTop:8,fontWeight:"bold"}}>Details:</Text></View>
      <View>
      {products.map((item, i) => (
        
      <ListItem key={i} bottomDivider>
      
        <ListItem.Content>
          <View style={{flexDirection:"row", flex:1, justifyContent:"space-between" }}>
          <TouchableOpacity>          
          <ListItem.Content>
          <Text>ID: {"          "+item.id}</Text>
          <Text>Name: {"    "+item.name}</Text>
          <Text>Quantity: {""+item.quantity}</Text>
          <Text>Color: {"      "+item.color}</Text>
          </ListItem.Content>
          </TouchableOpacity>
          </View>
          
        </ListItem.Content>
      </ListItem>
    ))}
      </View>
      </ScrollView>
   
    );
  }
}
class Products extends React.Component{
  render(){
    const products = [
      {
      id:444,
      name: 'Pencil',
      quantity: '10',
      color:"red"
      },
      {
      id:555,
      name: 'Marker',
      quantity: '30',
      color:"blue"
      },
    ]
    return (
      <ScrollView style={{backgroundColor:"white",flex:1}}>
      <View>
      {products.map((item, i) => (
      <ListItem key={i} bottomDivider>
        <ListItem.Content>
          <View style={{flexDirection:"row", flex:1, justifyContent:"space-between" }}>
          <TouchableOpacity onPress={()=>{this.props.navigation.navigate("Product Detail",products[i])}}>{i+1}{" "+item.name}</TouchableOpacity>
          </View>
          
        </ListItem.Content>
      </ListItem>
    ))}
      </View>
      </ScrollView>
    );
  }
}
class Orders extends React.Component{
  render(){
    const orders = [
      {
      oid:444,
      name: 'Pencil',
      quantity: '10',
      color:"red",
      price:"100/-",
      customerInformation:"Name: Ali, Address: Islamabad",
      orderDate:"11/12/20", 
      shippingStatus:"shipped",
      },
      {
      oid:555,
      name: 'Marker',
      quantity: '30',
      color:"blue",
      price:"200/-",
      customerInformation:"Name: Rubab, Address: Islamabad",
      orderDate:"11/12/20", 
      shippingStatus:"shipped",
      },
    ]
    return (
      <ScrollView style={{backgroundColor:"white",flex:1}}>
      <View>
      {orders.map((item, i) => (
      <ListItem key={i} bottomDivider>
      <TouchableOpacity>    
        <ListItem.Content>
          <View style={{flexDirection:"row", flex:1, justifyContent:"space-between" }}>
          <TouchableOpacity onPress={()=>{this.props.navigation.navigate("Order Detail",orders[i])}}>
          <Text>ID: {"           "+item.oid}</Text>
          <Text>Name: {"   "+item.name}</Text>         
          <Text>Price: {"      "+item.price}</Text>
          </TouchableOpacity>
          </View>
        </ListItem.Content>
        </TouchableOpacity>    
      </ListItem>
    ))}
      </View>
      </ScrollView>
    );
  } 
}
class OrdersDetails extends React.Component{
  render(){
    const orders=[this.props.route.params]
    return (
      <ScrollView style={{backgroundColor:"white",flex:1}}>
     <View style={{ backgroundColor:"orange",width:"33%",alignSelf:"center",marginTop:3}}><Text style={{fontSize:18,fontFamily:"Times New Roman",textAlign:"center",color:"white"}}>{this.props.route.params.name}</Text></View>
     <View><Text style={{marginLeft:8,marginTop:8,fontWeight:"bold"}}>Details:</Text></View>
      <View>
      {orders.map((item, i) => (
        
      <ListItem key={i} bottomDivider>
      
        <ListItem.Content>
          <View style={{flexDirection:"row", flex:1, justifyContent:"space-between" }}>
          <TouchableOpacity>          
          <ListItem.Content>
          <Text>ID: {"          "+item.oid}</Text>
          <Text>Name: {"    "+item.name}</Text>
          <Text>Quantity: {""+item.quantity}</Text>
          <Text>Color: {"      "+item.color}</Text>          
          <Text>Price: {"      "+item.price}</Text>
          <Text>ID: {"          "+item.customerInformation}</Text>
          <Text>Name: {"    "+item.orderDate}</Text>
          <Text>Quantity: {""+item.shippingStatus}</Text>
          </ListItem.Content>
          </TouchableOpacity>
          </View>
          
        </ListItem.Content>
      </ListItem>
    ))}
      </View>
      </ScrollView>
   
    );
  } 
}
class Employee extends React.Component{
  render(){
    const employees = [
      {
      eid:444,
      name: 'Ali',
      age: '30',
      designation:"Professor"
      },
      {
      eid:555,
      name: 'Amna',
      age: '39',
      designation:"Professor"
      },
    ]
    return (
      <ScrollView style={{backgroundColor:"white",flex:1}}>
      <View>
      {employees.map((item, i) => (
      <ListItem key={i} bottomDivider>
        <ListItem.Content>
          <View style={{flexDirection:"row", flex:1, justifyContent:"space-between" }}>
          <TouchableOpacity onPress={()=>{this.props.navigation.navigate("Employee Detail",employees[i])}}>
          <Text>Name: {"            "+item.name}</Text>
          <Text>Designation: {"  "+item.designation}</Text>
          </TouchableOpacity>
          </View>          
        </ListItem.Content>
      </ListItem>
    ))}
      </View>
      </ScrollView>
    );
  } 
}
class EmployeeDetails extends React.Component{
  render(){
    const employees=[this.props.route.params]
    return (
      <ScrollView style={{backgroundColor:"white",flex:1}}>
     <View style={{ backgroundColor:"orange",width:"33%",alignSelf:"center",marginTop:3}}><Text style={{fontSize:18,fontFamily:"Times New Roman",textAlign:"center",color:"white"}}>{this.props.route.params.name}</Text></View>
     <View><Text style={{marginLeft:8,marginTop:8,fontWeight:"bold"}}>Details:</Text></View>
      <View>
      {employees.map((item, i) => (
        
      <ListItem key={i} bottomDivider>
      
        <ListItem.Content>
          <View style={{flexDirection:"row", flex:1, justifyContent:"space-between" }}>
          <TouchableOpacity>          
          <ListItem.Content>
          <Text>ID: {"          "+item.eid}</Text>
          <Text>Name: {"    "+item.name}</Text>
          <Text>Quantity: {""+item.age}</Text>
          <Text>Color: {"      "+item.designation}</Text>
          </ListItem.Content>
          </TouchableOpacity>
          </View>
          
        </ListItem.Content>
      </ListItem>
    ))}
      </View>
      </ScrollView>
   
    );
  } 
}
class Home extends React.Component{
  render(){
    return (
      <View style={{flex:1,backgroundColor:"white",marginBottom:"18%", marginTop:"18%"}}>
        <View style={styles.home}>
        <View style={{ marginTop:"19%",marginLeft: "28%",width:"33%"}}>
          <BTN width={"150%"} color={"orange"} title={'Manage Product'} textcolor={"white"} event={()=>{this.props.navigation.navigate("Products")}}/>
        </View> 
        <View style={{marginTop:"10%",marginLeft: "28%",width:"33%"}}>
          <BTN width={"150%"} color={"orange"} title={'Manage Employee'} textcolor={"white"} event={()=>{this.props.navigation.navigate("Employee")}}/>
        </View>
        <View style={{marginTop:"10%",marginLeft: "28%",width:"33%"}}>
          <BTN width={"150%"} color={"orange"} title={'Manage Orders'} textcolor={"white"} event={()=>{this.props.navigation.navigate("Orders")}}/>
        </View>
        </View>       
      </View>
    );
  }
}
const Stack = createStackNavigator();
export default class App extends React.Component{
  
  render(){
    return (
      <NavigationContainer>
      <Stack.Navigator
      screenOptions={{
        headerTitleAlign:"center",
         headerTintColor:"white",
         headerStyle:{
           backgroundColor:"orange",
           borderWidth:2,
          borderColor:"#3A4655",
         },
      }}
      >
        <Stack.Screen name="Home" component={Home}/>
        <Stack.Screen name="Products" component={Products}/>
        <Stack.Screen name="Product Detail" component={ProductDetails}/>
        <Stack.Screen name="Employee" component={Employee}/>
        <Stack.Screen name="Employee Detail" component={EmployeeDetails}/>
        <Stack.Screen name="Orders" component={Orders}/>
        <Stack.Screen name="Order Detail" component={OrdersDetails}/>
        </Stack.Navigator>
      </NavigationContainer>  
    );
  }
 
}

const styles = StyleSheet.create({
  home: {
    marginTop:"10%",
    backgroundColor: 'white',
  },
  paragraph: {
    margin: 24,
    fontSize: 18,
    fontWeight: 'bold',
    textAlign: 'center',
  },
});


