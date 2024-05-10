# Function: index()

```ts
function index<IndexerOptions>(params: {
  "documents": {
     "content": ({
        "media": undefined;
        "text": string;
       } | {
        "media": {
           "contentType": string;
           "url": string;
          };
        "text": undefined;
       })[];
     "metadata": Record<string, any>;
    }[];
  "indexer": IndexerArgument<IndexerOptions>;
  "options": TypeOf<IndexerOptions>;
}): Promise<void>
```

Indexes documents using a [IndexerAction](../type-aliases/IndexerAction.md) or a DocumentStore.

## Type parameters

| Type parameter |
| :------ |
| `IndexerOptions` *extends* `ZodType`\<`any`, `any`, `any`, `IndexerOptions`\> |

## Parameters

| Parameter | Type |
| :------ | :------ |
| `params` | `object` |
| `params.documents` | \{ `"content"`: (\{ `"media"`: `undefined`; `"text"`: `string`; \} \| \{ `"media"`: \{ `"contentType"`: `string`; `"url"`: `string`; \}; `"text"`: `undefined`; \})[]; `"metadata"`: `Record`\<`string`, `any`\>; \}[] |
| `params.indexer` | `IndexerArgument`\<`IndexerOptions`\> |
| `params.options`? | `TypeOf`\<`IndexerOptions`\> |

## Returns

`Promise`\<`void`\>

## Source

[ai/src/retriever.ts:234](https://github.com/firebase/genkit/blob/9cb10ef63dd6659f1a31ffd2367b7efa8acc10e5/js/ai/src/retriever.ts#L234)