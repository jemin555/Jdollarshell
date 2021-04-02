
 J$shell
=========

J$shell is  a programming language invented by wilmix jemin at years 2014,2019 and it  is used with  writ technologies.
ie) J$shell Project took place  between Jan 2014 to  Feb 2019...

J$shell supports Obfuscuation, prevents code stealing.
J$Shell p.l  also  comes with J$shell CWE-Editor.
J$Shell p.l is invented in Gdollar p.l and Java.
but J$ShellCWEEditor is invented in C#.
J$Shell program also  connect  with  Wnosql(*) Securable Database

SYNTAX for J$Shell 
==================

<JSHELL>

<USE> package;
<PACK> packagename
<%
    <CLASS> classname
    {
        public void main()
        {
         
<$ J$shell source code %>
 
  


%>

?>



ABOUT J$Shell
================

J$shell contains J$Shell-Cdollar Advanced DataStructures,C/C++ oops called  as  J$shell oops.

J$Shell also  be  used to create  datastructures..

J$Shell also contains  J$C$Shellpackages.. So no need  to study CDollar p.l.




Example-1 :Write  a  J$Shell program using pointer
========   ======================================= 


<Jshell>
<PACK> MyP
{
    <CLASS> Programs
    {
        public void main()
        {
            

	<Str>  s="dsdds";

// pointer {*} pointer name (l) Pointers ( variablevalue) 
		
		{*} l Pointers (s);  
// add s value to Pointer l		
l.add(s);
		
		for (int i = 0; i NOT= l.size(); i = i + 1)
		{
		
		<OBJECT> obj=l.GETKEY(i);
			<PRINTLN>(obj);
			
			
			
		}
		
		
              
                
               
     %>

?>

Output:
=======

dsdds
dsdds

NOTE:When you compile the  program  using J$SHELL-CWEEDITOR you will get pointer.Jshell object file

and  *.exe and  *.dll file  in  output folder.

==================================================================================================
Example-2 : Write a J$Shell program  using J$Shelloops concepts  BAG for constructing Tree.
===========


<Jshell>

<USE> CUTIL;
<PACK> HierachialTree
<%
    <CLASS> roots
    {
        public void main()
        {
         

 Bag  tree <NEW> Bag();
 
  Bag  Member <NEW> Bag();

       
Member.PUT("A","CLASS5");
Member.PUT("B","CLASS5");
Member.PUT("C","CLASS5");
Member.PUT("D","CLASS5");
Member.PUT("CLASS6","CLASS6");
 Bag  slibings <NEW> Bag();
slibings.PUT("A","s1");
slibings.PUT("A","s2");
slibings.PUT("B","s11");
slibings.PUT("B","s21");
slibings.PUT("C","s12");
slibings.PUT("C","s22");
Bag  activity <NEW> Bag();
activity.PUT("s1","cricket");
activity.PUT("s2","read");
activity.PUT("s21","swim");
activity.PUT("s12","swim");
tree.PUT(1,Member);
tree.PUT(2,slibings);
tree.PUT(3,activity);


activity.remove("s1","cricket");
tree.remove(3,activity);
tree.PUT(3,activity);



<PRINTLN>("output="+tree.containsValue(Member));
              
  <PRINTLN>("outputTree="+tree);
   


%>

?>

output
======

output=True
outputTree={1=[{A=[CLASS5], B=[CLASS5], C=[CLASS5], D=[CLASS5], CLASS6=[CLASS6]}], 2=[{A=[s1, s2], B=[s11, s21], C=[s12, s22]}], 3=[{s2=[read], s21=[swim], s12=[swim]}]}





Example-3: Create a  employee table, list the  employee table, insert some values into employee table, update the name "shyam"  to "Sriram" using JSHELL program
==========   ==================================================================================================================================================== 

<Jshell>

<USE> WDBA;
<USE> CDollar.WDBA;

<USE> CUTIL;


<PACK> ConsoleApplication1
{
    <CLASS> Program
    {
        public void main()
        {




            String g = WDBASQL.WDBASQLS("datastores", "USEDATABASE", "dbpwds", "C:\\Programs\\WNOSQL\\WNOSQLProgramfiles\\WNOSQL-cod");


            String t = WDBASQL.WDBASQLS("dbuser", "dbpwds", 1, "wilmix78", "wilmix78", 1, 5, g);

            String s1 = "CREATETABLE from Employee 0 to 0 , 1 to 6 ?= X By 1 1 : {ENO,ENAME,DESIGNATION,SALARY}: {0} :{0}";

          <PRINTLN>("" + WDBALIB.WDBAQUERY(s1, t));



            String s11 = "SELECTRVAL from Employee 0 to 0 , 1 to 6 ?= X By 1 1 : {0} : {0} :{0}";


            <PRINTLN>("" + WDBALIB.WDBAQUERY(s11, t));



            String s12 = "INSERTINTO from Employee 4 to " + WDBALIB.WDBAQUERY(s11, t).size() + " , 1 to 6 ?= X By 1 1 : {0} : {2,jemin,sse2,300000,3,shyam,mgr,500000} : {0}";


            <PRINTLN>("" + WDBALIB.WDBAQUERY(s12, t));


            String s112 = "SELECTRVAL from Employee 0 to 0 , 1 to 6 ?= X By 1 1 : {0} : {0} :{0}";


            <PRINTLN>("" + WDBALIB.WDBAQUERY(s112, t));



            String s171 = "UPDATE from Employee 0 to 0 , 1 to 6 ?= C By 1 1 : {shyam} :{sriram}:{0}";
            <PRINTLN>("" + WDBALIB.WDBAQUERY(s171, t));

            


%>

?>

Output
======



[ENO ENAME DESIGNATION SALARY]

 Listing Table  Employee contents ...

IP=1

-------------


-------------


-------------


-------------

        [ENO |           ENAME |                 DESIGNATION |           SALARY] |
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

        [ENO |           ENAME |                 DESIGNATION |           SALARY |                0] |


[ENO ENAME DESIGNATION SALARY 0][]


[ENO, ENAME, DESIGNATION, SALARY, 0, 2, jemin, sse2, 300000, 3, shyam, mgr, 500000]

Table  updated  sucessfuly 


[ENO, ENAME, DESIGNATION, SALARY, 0, 2, jemin, sse2, 300000, 3, sriram, mgr, 500000]













