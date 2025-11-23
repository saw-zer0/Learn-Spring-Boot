## List Methods 
`.stream()`
`.map()`
`.collect(Collector.toList())`

## Optional Class
- Optional type and prevent common NullPointerException (NPE) errors
- Can be used with `.orElse()`
- If your query logic ensures that only zero or one result will be returned (e.g., searching by a unique field like email or username), you should declare the return type as `Optional<T>`.

## Lombok 
### Annotations
- `@Getter`
- `@Setter`
- `@NoArgsConstructor`
- `@AllArgsConstructor`
- `@Data` - Combo of Getter Setter and Required Args Constructor
- `@Builder` - Implement Builder Design pattern
- `@SuperBuilder`
- `@EqualsAndHashCode`
-

## Faker


## Random Java Things
- `implements Serializable` - 