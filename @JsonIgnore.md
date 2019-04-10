java
``
public Car {

  @JsonIgnore
  private String currentSpeed;
  private String maxSpeed;
  
  @Override
  public String toString() {
        return "Car{" +
                "currentSpeed=" + currentSpeed +
                ", maxSpeed='" + maxSpeed + '\'' +
                '}';
    }
  
}
``
