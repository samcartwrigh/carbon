## A Flash widget.

The flash is rendered in two sections: a ventral message 'flash', and a
dorsal coloured, expanding 'slider'.

### How to use an Flash in a component:

In your file:

```js
  import Flash from 'carbon/lib/components/flash';
```

To render a Flash, setup open and cancel handlers in your view to trigger
the message on and off:

```js
 <Flash open={ openStatus } onDismiss={ myOnDismiss } message='Alert!' />
```

By default, the flash renders with a clickable close icon that hooks up with the onDismiss function.
To instead have the flash disappear after a given time period, pass a prop of timeout in milliseconds.

```js
 <Flash open={ openStatus } onDismiss={ myOnDismiss } message='Alert!' timeout={ 2000 }/>
```