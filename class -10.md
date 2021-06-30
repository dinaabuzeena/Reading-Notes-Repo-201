# BASIC MAP SETTINGS
# CREATING A MAP
The maps object is stored within an object called googl e. This creates scope for all Google objects.
To add a map to your page, you create a new map object using a constructor: Map (). The constructor is
part of the maps object, and it has two parameters: 
• The element into which you want the map drawn
• A set of map options that control how it is displayed given using object literal notation 

# MAP OPTIONS
The settings that control how the map should look are stored inside another JavaScript object called
mapOpti ons. It is created as an object literal before you call the Map() constructor. In the JavaScript on
the right, you can see that the mapOpt ions object uses three pieces of data:
• Longitude and latitude of the center of the map
• The zoom level for the map
• The type of map data you want to show
 c09/google-map. html


<div id="map"></div>
<script src="js/google-map.js"></ script>
</body> 
function ini t() {
,
var mapOpt ions = { // Set up the map options
center: new google .maps.Latlng(40 . 782710,-73 .965310),
mapType!d: google .maps.MapType ld.ROADMAP,
zoom: 13
} ;
~ var venueMap; // Map() draws a map
~ venueMap =new google .maps.Map(document .getElementByld('map'), mapOptions} ;
2
}
function l oadScript() {
va r scri pt document . createEl ement('script '); // Create <script> element
scri pt .sr c = 'http://maps.googl eapis. com/maps/api/js?
sensor=false&callback= i nitial ize ' ;
document.body. appendChi l d(scri pt) ; //Add element to page
G) window. on 1 oad 1 oadScri pt; // Onload call 



# Erorr Handling
JavaScript can be hard to learn and everyone makes mistakes when writing it. This chapter will help you learn
how to find the errors in your code. It will also teach you how to write scripts that deal with potential errors gracefully. When you are writing JavaScript, do not expect to write it perfectly the first time.
Programming is like problem solving: you are given a puzzle and not only do you have to solve it, but you also need to create the instructions that allow the computer to solve it. too


# ORDER OF EXECUTION
To find the source of an error, it helps to know how scripts are processed.
The order in which statements are executed can be complex; some tasks cannot complete until another statement or function has been run:

# EXECUT.ION CONTEXTS 
The JavaScript interpreter uses the concept of execution contexts.
There is one global execution context; plus, each function creates a new new execution context. They correspond to variable scope. 

# EXECUTION CONTEXT & HOISTING
1: PREPARE
• The new scope is created
• Variables, functions, and arguments are created
• The value of the this keyword is determined 

2: EXECUTE
• Now it can assign values to variables
• Reference functions and run their code
• Execute statements


# ERROR OBJECTS CONTI NUED

# Syntax Error
SYNTAX IS NOT CORRECT
This is caused by incorrect use of the rules of the
language. It is often the result of a simple typo.
MISMATCHING OR UNCLOSED QUOTES
document .write ("Howdyl );
SyntaxError: Unexpect ed EOF
MISSING CLOSING BRACKET
document .getElementByid('page' I
SyntaxErr or : Expected token ' ) '
MISSING COMMA IN ARRAY
Would be same for missing] at the end
var l ist = ['Item 1', 'Item 2 ' l 'rtem 3'];
SyntaxError: Expected token ']'
MALFORMED PROPERTY NAME
It has a space but is not surrounded by quote marks
user = {f i rstl name: "Ben", lastName: "Lee"};
Synt axError: Expected an identifier but
found 'name ' instead 


# Ref erenceError
VARIABLE DOES NOT EXIST
This is caused by a variable that is not declared or is
out of scope.
VA RIABLE IS UNDECLARED
var wi dth = 12 ;
var area = width * llt!ftNU! ;
ReferenceError: Can ' t find vari able:
height
NAMED FUNCTION IS UNDEFINED
document.write ( randomFunction() ) ;
ReferenceError: Can't find variable :
randomFunction

# Ev alError
INCORRECT USE OF eval() FUNCTION
The eva l () function evaluates text through the
interpreter and runs it as code (it is not discussed
in this book). It is rare that you would see this type
of error, as browsers often throw other errors when
they are supposed to throw an Eva 1 Error. 


# UR I Error
INCORRECT USE OF URI FUNCTIONS
If these characters are not escaped in URls, they will
cause an error: / ? & I : ;
CHARACTERS ARE NOT ESCAPED
decodeURI('http: //bbc . com/ news . phplla=l');
URlError: URI error