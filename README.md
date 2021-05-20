# JSInterviewQuestions

var myObject = {
    foo: "bar",
    func: function() {
        var self = this;
        console.log("outer func:this.foo= " + this.foo);
        console.log("outer func:self.foo= " + self.foo);
        (function() {
            console.log("inner func: this.foo= " + this.foo);
            console.log("inner func:  self.foo= " + self.foo);
        }());
    }
};
myObject.func();

console.log(1 +  "2" + "2");
console.log(1 +  +"2" + "2");
console.log(1 +  -"1" + "2");
console.log(+"1" +  "1" + "2");
console.log( "A" - "B" + "2");
console.log( "A" - "B" + 2);





var a = { 'id':3,'name':'s'}
var b=a;
b['id']=3;
console.log(a);
console.log(b);
var x = 21;
var girl = function () {
    console.log(x);
    var x = 20;
};
girl ();
var b = 1;
function outer(){
   	var b = 2
    function inner(){
        b++;
        var b = 3;
        console.log(b)
    }
    inner();
}
outer();
var hero = {
    _name: 'John Doe',
    getSecretIdentity: function (){
        return this._name;
    }
};

var stoleSecretIdentity = hero.getSecretIdentity;

console.log(stoleSecretIdentity());
console.log(hero.getSecretIdentity());
var list = readHugeList();

var nextListItem = function() {
    var item = list.pop();

    if (item) {
        // process the list item...
        nextListItem();
    }
};
var a=[1,2,3]
a[10]=99;
a[6];
a[4]
https://medium.com/the-clever-dev/50-difficult-javascript-interview-questions-88e6e92367e7
