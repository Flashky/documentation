
```java
public Car {

  @JsonIgnore
  private Integer currentSpeed;
  private Integer maxSpeed;
  
  public Integer getCurrentSpeed() {
    return currentSpeed;
  }
  
  public void setCurrentSpeed(Integer currentSpeed) {
    this.currentSpeed = currentSpeed;
  }
  
  public Integer getMaxSpeed() {
    return maxSpeed;
  }
  
  public void setMaxSpeed(Integer maxSpeed) {
    this.maxSpeed = maxSpeed;
  }
  
  @Override
  public String toString() {
        return "Car{" +
                "currentSpeed=" + currentSpeed +
                ", maxSpeed='" + maxSpeed + '\'' +
                '}';
    }
  
}
```
