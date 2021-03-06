---
kind: FunctionDeclaration
name: ɵɵattributeInterpolate2
module: core
---

# ɵɵattributeInterpolate2

## description

Update an interpolated attribute on an element with 2 bound values surrounded by text.

Used when the value passed to a property has 2 interpolated values in it:

```html
<div attr.title="prefix{{v0}}-{{v1}}suffix"></div>
```

Its compiled representation is::

```ts
ɵɵattributeInterpolate2("title", "prefix", v0, "-", v1, "suffix");
```

```ts
function ɵɵattributeInterpolate2(
  attrName: string,
  prefix: string,
  v0: any,
  i0: string,
  v1: any,
  suffix: string,
  sanitizer?: SanitizerFn,
  namespace?: string
): typeof ɵɵattributeInterpolate2;
```

[Link to repo](https://github.com/timdeschryver/angular/blob/master/packages/core/src/render3/instructions/attribute_interpolation.ts#L81-L94)

## Parameters

| Name      | Type          | Description                               |
| --------- | ------------- | ----------------------------------------- |
| attrName  | `string`      | The name of the attribute to update       |
| prefix    | `string`      | Static value used for concatenation only. |
| v0        | `any`         | Value checked for change.                 |
| i0        | `string`      | Static value used for concatenation only. |
| v1        | `any`         | Value checked for change.                 |
| suffix    | `string`      | Static value used for concatenation only. |
| sanitizer | `SanitizerFn` | An optional sanitizer function            |
| namespace | `string`      |                                           |

## returns

itself, so that it may be chained.

## codeGenApi
