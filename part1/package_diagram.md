```mermaid
classDiagram
class PresentationLayer {
    <<Interface>>
    +ServiceAPI


}
class BusinessLogicLayer {
    +User
    +Place
    +Review
    +Amenity
}
class PersistenceLayer {
    +DatabaseAccess
    +Repository

}
PresentationLayer --> BusinessLogicLayer : Facade Pattern
BusinessLogicLayer --> PersistenceLayer : Database Operations
