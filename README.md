# SS7-Attack
knowledge about SS7 attack and hack
SS7 Hack or SS7 Attack :

SS7 hack or signaling system 7 hack is the process of getting calls or sms for a subscriber, getting on another mobile number or in an application. These days many applications uses confirmation of a user identity from sms or voice call. . If some how call and sms routed to another number then its possible to hack. In this ss7 hack tutorial, the ss7 protocol and call flows will be explained. The Hack tutorial covers the call and sms hacking.

Ss7 vulnerability, exposes the network for sms and voice hack.  Along with this , once access to ss7 network, the real time location of a person can be obtained.

SS7 is the traditional network which uses standard ISUP and MAP protocol for call and sms.

SS7 hack is not  simple as it looks, people claims to install a software and then just enter phone number to hack sms or calls.  Getting calls and sms via hack, is the process to connect to ss7 network and run an application, so that the home network of original subscriber gets impression that software is the roaming VLR/MSC node in a network. The fist step is to get the ss7 connection.
Get a SS7 Connection for hack:

Get SS7 Global Title and Point Code : For a SS7 connection , one should have a Global Title and a point code (international) , a local point code (local, between you and mobile operator )can be used, depends on ss7 connection provider. If one is a  mobile operator , then  get this from standard GSM body . A new network code is assigned by gsm , so that you can have big range of global titles or MSISDNs and IMSIs.

If not a mobile operator, one can take global title on lease from a mobile operator. Once you have GT , now there are following options.

SS7 connection via an aggregator: In this you can connect to a SS7 agrregator and they can publish you GT, on all networks. So any traffic coming to your GT , will be forwarded by aggregator towards your node or application. Mostly MVNO does this , they have GT ranges, those are published to aggregator for connecting mobile network operators globally.

Directly with a Mobile Operator: In this you will have direct links with mobile operators , each will set routing for your GT , towards the serving node. In this you need to connect each mobile operators Individually.

SS7 vs Sigtran:

If you are using pure SS7 (E1/T1), then the box with application should be in premises of a mobile operators. If using sigtran, which is IP based, You can have your box in data center on cloud.
Ss7 hack tool or Software:

Once one have ss7 connection. Now time for a develop a ss7 application for GSM MAP signaling. Sdk for ss7 provides required ss7 stack and libraries for developing ss7 hack software.  Before developing application first finalize the requirements.  If one want to receive sms , than application should  be develop to handle protocol messages for sms. Now the ss7 application will simulates as it is a real device.
Application Registration as a real phone:

The first step is to register the application as a phone registers in roaming network. This required the IMSI of the sim card , to which the mobile number belongs.  Mobile number every one have but IMSI don't . So the first step is to get IMSI. Hacking Application sends SRI-SM with phone number to the hlr, which sends IMSI and roaming information in response. Roaming information includes the county code and area code.

From IMSI the application build the location update along with other parameter. The open a TCAP dialogue to the SS7 node. The open dialogue needs to fill SCCP called party address and SCCP Calling party address. Called Party address is derived from IMSI and calling party address is the GT of software application.

During Update Location, HLR will  respond with ISD or Insert Subscriber Data. Software application needs to acknowledge the ISD to the HLR , else update location procedure will fail and application will not attach as phone.  One HLR sends update location ACK, means registration is done.
SS7 Hack for sms:

Once the application registered with the home network. When request for authentication sms starts. The global title of ss7 hack software updated on the home HLR as a outcome of update location call flow. When request for authentication sms starts. HLR gets SRI-SM query, the response of SRI-SM , have visiting MSC number. In this case the MSC number is the GT of application. The sender sms will send the sms to the software application. Now its applications responsibility to decode the message and display the message a string. Now you have the authentication code you were looking for.
SS7 Hack for Voice: 

For voice , after phone registration call flow. The hack software should activate the call forwarding to the new number. While activating call forwarding, the ss7 hack tool can send the type of call forwarding and the mobile number where the hacker want to receive the call.  The call forwarding type can be "Call Forwarding Unconditionally". This will enable call forwarding all the time.  In this case even the mobile user never come to know that his call has been hacked. After voice verification the call forwarding can be removed.
SS7 hack applications examples:

Any application which which required user verification from sms or voice can be hacked by the ss7 network. We will cover the ss7 call flows for WhatsApp and Facebook.
ss7 hack whatsapp:

Whatsapp is used every where. It does messaging and file transfer over ip network. It connects you phone book to the others using phone numbers. So no need to add a contact explicitly.  Like in skype, we need to create an account and need to add others skype ids before any communication. But with this app, the phone number is the profile id.  While installing whatsApp it requires  user authentication via SMS.  If WhatsApp needs to hack, after installation, run the ss7 hack software app and received the authentication message on the hack software app.  Enter the code in installed WhatsApp. Now you can have messages on your WhatsApp, while the number belongs to other guy.
