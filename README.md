# LYM-p3
---------------------------------
EJEMPLO QUE FUNCIONA:
---------------------------------

defVar nom 0
defVar x 0
defVar y 0
defVar one 0
defProc putCB (c , b )
{ 
	drop( c ) ; 
	letGo ( b ) ;
	walk( n ) 
	
}
defProc goNorth ()
{
	while can(walk(1 , north ) ) { walk(1 , north ) } 
}
defProc goWest ()  
{
	if can(walk(1 , west ) ) { walk(1 , west ) } else {nop ()}
}
 {
	jump (3 ,3) ;
	putCB (2 ,1)
}
$
---------------------------------
EJEMPLO QUE NO FUNCIONA:
---------------------------------

defVar nom 0
defVar x 0
defVar y 0
defVar one 0
defProc putCB (c , b )
{ 
	drop( c ) ; 
	letGo ( b ) ;
	walk( n ) 
	
}
defProc goNorth ()
{
	while can(walk(1 , north ) ) { walk(1 , north ) } 
  defProc goWest ()  
  {
	  if can(walk(1 , west ) ) { walk(1 , west ) } else {nop ()}
  }

}
{
	jump (3 ,3)
	putCB (2 ,1)
}
$