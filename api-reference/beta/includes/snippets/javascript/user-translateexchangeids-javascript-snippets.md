---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1709999f9cbbb09e1e44ef73a2ff9785910acafad1289ef3fd8b33ec09f28572
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164136"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const convertIdResult = {
  inputIds: [
    '{rest-formatted-id-1}',
    '{rest-formatted-id-2}'
  ],
  sourceIdType: 'restId',
  targetIdType: 'restImmutableEntryId'
};

await client.api('/me/translateExchangeIds')
    .version('beta')
    .post(convertIdResult);

```