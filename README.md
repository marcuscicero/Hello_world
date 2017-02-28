# Hello_world
gdrstghsths
fsrgdrgd
rgddrgerd
drgfgd
public class Ship {

	
	
	//1
	
	
	private double Xcoordinate;
	private double Ycoordinate;
	private double velocity_x;
	private double velocity_y;
	private double orientation;
	private double radius;
	
	public Ship(double Xcoordinate,double Ycoordinate,double velocity_x,double velocity_y, double orientation,double radius) {
		setXcoordinate(Xcoordinate);
		setYcoordinate(Ycoordinate);
		setVelocity_x(velocity_x);
		setVelocity_y(velocity_y);
		setOrientation(orientation);
		setRadius(radius);
		
		
	}

	public double getYcoordinate() {
		return Ycoordinate;
	}

	public void setYcoordinate(double ycoordinate2) {
		Ycoordinate = ycoordinate2;
	}

	
	public double getXcoordinate() {
		return Xcoordinate;
	}

	public void setXcoordinate(double xcoordinate) {
		Xcoordinate = xcoordinate;
	}

	public double getVelocity_x() {
		return velocity_x;
	}

	public void setVelocity_x(double velocity_x) {
		this.velocity_x = velocity_x;
	}

	public double getVelocity_y() {
		return velocity_y;
	}

	public void setVelocity_y(double velocity_y) {
		this.velocity_y = velocity_y;
	}
	public double getVelocity(){
		return Math.sqrt(Math.pow(this.getVelocity_x(),2)+Math.pow(this.getVelocity_y(),2));
		
	}
	public double getOrientation() {
		return orientation;
	}

	public void setOrientation(double orientation) {
		this.orientation = orientation% (2*Math.PI);
	}

	public double getRadius() {
		return radius;
	}

	public void setRadius(double radius) {
		this.radius = radius;
	}
	
	
	//2
	
	public void move(double time) {
		
	}
	public void turn (double angle){
		
	}
	public double getMaxspeed() {
		return 300000;
				
	}

	public void thrust (double a){
		if (a<0);
			a=0;
		setVelocity_x(this.getVelocity_x()+a*Math.cos(this.getOrientation()));
		setVelocity_y(this.getVelocity_y()+a*Math.sin(this.getOrientation()));
		if (this.getVelocity()>getMaxspeed());
			
		
	}
	
	//3 defensief
	
	public Ship getDistanceBetween( Ship other){
		return other;
		
	}
	public boolean overlap( Ship other){
		return true;
		
	}
	public Ship getTimeToCollision( Ship other){
		return other;
	}
	
	public Ship getCollisonPosition(Ship other){
		return other;
	}
	
	
	
	
	
	
