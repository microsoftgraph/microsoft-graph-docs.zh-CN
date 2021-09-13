---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a83ccc7db632b4c6e5e8a2a9bae935220d8580d089cee86bf2f3d0ccb66c1584
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277487"
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
    .post(convertIdResult);

```