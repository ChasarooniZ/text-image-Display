# text-image-Display

Paste in results of this into the text input to get the item descriptions price and amt.

// Note need to have actor you want info on selected (built for 5e)

_token.actor.items.filter(i => i.type !== 'feat' && i.type !== 'spell' && i.type !== 'class' && i.type !== 'background' && i.type !== 'subclass').map(e => ({name: e.name, desc: e.system.description.value, price: `${e?.system?.price?.value} ${e?.system?.price?.denomination}`, amt: e.system.quantity}))
