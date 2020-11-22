# Challenge 6 : Frame Development

1. Node Template : Update Pallet template to include a storage item for a custom struct.Add at least one dispatchable function to interact with the new storage
item.

Struct

```
pub struct Opinion{
	name: Vec<u8>,
	email: Vec<u8>,
	comment: Vec<u8>,
}

```

Added enter_opinion() to store user input.

2. Front End Template : Add the necessary types to interact with the dispatchable.

Types added in https://github.com/encoderafat/framedev/blob/main/substrate-front-end-template/src/substrate-lib/SubstrateContext.js

```
types: { ...config.CUSTOM_TYPES, Opinion: { name: 'Vec<u8>', email: 'Vec<u8>', comment: 'Vec<u8>' } },

```

<img src="https://github.com/encoderafat/framedev/blob/main/img/enteropinion.jpg" />

name, email and comment map to name, email and comment keys of the struct Referendum.

<img src="https://github.com/encoderafat/framedev/blob/main/img/opinionstatus.jpg" />

Querying the saved struct values.
