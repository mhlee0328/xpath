# XPathResult interface

Represents the result of an XPath expression. This interface is used for the parameters passed into custom functions
used in [function resolvers](function resolvers.md) and can represent a number, a string, a boolean value, or a node set.

## Methods and Getters

```typescript
booleanValue: boolean;
```

Returns the boolean value of the result in accordance with the XPath 1.0 spec.

```typescript
numberValue: number;
```

Returns the numeric value of the result in accordance with the XPath 1.0 spec.

```typescript
stringValue: string;
```

Returns the string value of the result in accordance with the XPath 1.0 spec.

## Methods and properties that are only present on `XPathResult`s representing node sets

```typescript
toArray(): Node[]
```

Returns an array of the nodes in the node set, in document order.

```typescript
first(): Node
```

Returns the first node in the node set, in document order.

```typescript
size: number;
```

Returns the number of nodes in this node set
