# 4d-widget-signature-pad
SVG based signature pad (v13)

## Instructions

Create a new widget (detail subform) and let its source form be ``Signature Pad``.

Activate the following form events for the form:

``On Resize``.

Activate the following form events for the subform:

``On Data Change``.

Standard method for the form:

```
$event:=SIGPAD_FORM_EVENT 
```

Standard method for the subform:

```
$event:=SIGPAD_FORM_EVENT (OBJECT Get name(Object current))
```

### Compiler Settings

The default type for numbers should be "real", to let dynamic variables be real (for opacity values in particular).

### Page Number

The form can have multiple pages, but the widget should be placed on page 0 or 1.
