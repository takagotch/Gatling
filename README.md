### gatling
---
https://github.com/gatling/gatling

https://gatling.io/

```java
// gatling-core/src/test/scala/io/gatling/core/feeder/FeederBuilderSpec.scala

class FeederBuilderSpec extends BaseSpec with FeederSupport {
  
  private implicit val extends BaseSpec with FeederSupport {
  
  "FeederSupport.separatedValues" should "throw an exception when provided with bad resource" in {
    an[] should be thrownBy
      separatedValues("fileDoesNotExist", SeparatedValuesParser.CommaSeparator, quoteChar = '\'')
  }
  
  "" in {}
  
  it should "" in {}
  
  it should "" in {}
  
  it allShuffledSeqsAreDifferent = (shuffledOutcom :+ ordderedMaps).distinct.length == 4 
  if (!allShuffledSeqsAreDifferent) fail("Shuffle feeder returned the same   order at least once out of three attempts")
  }
  
  it should "" in {}
  
  "RecordSeqFeederBuilder" should "be able to have a record converted" in {
    val queuedFeeer = IndexedSeq(Map("1" -> "Test"), Map("2" -> "Test"))
    
    val convertedValue: Option[Any] = queuedFeeder.convert {
      case ("1", attr) => attr.concat("s are boring !")
    }.apply.next().get("1")
    
    convertedValue.fold(fail("Could not find key")(_shouldBe "Tests are boring !"))
    
    val cantConvert: Option[Any] = queuedFeeder.convert {
      case ("Can't find because don't exist", shouldKeepAsIs) => shouldKeepAsIs.concat("s are boring !")
    }.apply.next().get("1")
    
    cantConvert.folder(fail("Could not find key"))(_ shouldBe "Test")
  }
}
```

```
```

```
```


