# Lucia

Lucia is an open source auth library that abstracts away the complexity of handling sessions. It works alongside your database to provide an API that's easy to use, understand, and extend.

- No more endless configuration and callbacks
- Fully typed
- Works in any runtime - Node.js, Bun, Deno, Cloudflare Workers
- Extensive database support out of the box

```ts
import { Lucia } from "lucia";

const lucia = new Lucia(new Adapter(db));

const session = await lucia.createSession(userId, {});
await lucia.validateSession(session.id);
```

*Logo by [@dawidmachon](https://github.com/dawidmachon), licensed under [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/).*

## Related libraries

- [Oslo](https://github.com/pilcrowonpaper/oslo)
- [Arctic](https://github.com/pilcrowonpaper/arctic)
