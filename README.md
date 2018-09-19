import javax.swing.*;
import javax.swing.plaf.synth.SynthTextAreaUI;

public class Invoice {
    String password;
    String consecutiveNumber;
    String emissionDate;
    String transmitterName;
    String transmitterLastName;
//  String idType;
//  String tradeName;
    String location;

    String receiverName;
    String receiverLastName;
//  String saleCondition;
    String creditTimeFrame;
//  String paymentMethod;
//  String serviceDetails;
    String summaryInvoice;




//   String d{50,50}

    public void setPassword(String password){
        this.password = password;
    }

    public String getPassword(){
        return password;
    }

//    String d{20,20}"

    public void setConsecutiveNumber(String consecutiveNumber){
        this.consecutiveNumber = consecutiveNumber;
    }

    public String getConsecutiveNumber(){
        return consecutiveNumber;

    }

//    datetype

    public void setEmissionDate(String emissionDate){
        this.emissionDate = emissionDate;
    }

    public String getEmissionDate(){

        return emissionDate;
    }

    // max 80 chars
    public void setTransmitterName(String name, String lastName){
        this.transmitterName = name;
        this.transmitterLastName = lastName;
    }

    public String getTransmitterName(){
        return transmitterName + " "  + transmitterLastName;
    }

//    minOcurs  = 0

    public void setReceiverName(String name, String lastName){
        this.receiverName = name;
        this.receiverLastName = lastName;
    }

    public String getReceiverName(){
        return receiverName + " "  + receiverLastName;
    }


//   minOccurs="0" / String maxLength 10

    public void setCreditTimeFrame(String creditTimeFrame){
        this.creditTimeFrame = creditTimeFrame;
    }

    public String getCreditTimeFrame(){
        return creditTimeFrame;
    }

}
