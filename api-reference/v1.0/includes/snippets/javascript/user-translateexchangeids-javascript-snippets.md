---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a9478571a989819c105c1f56e2259ae2554da7c5
ms.sourcegitcommit: 997fbfe36b518e0a8c230ae2e62666bb5c829e7e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/19/2019
ms.locfileid: "37041901"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const convertIdResult = {
  "inputIds" : [
    "{rest-formatted-id-1}",
    "{rest-formatted-id-2}"
  ],
  sourceIdType: "restId",
  targetIdType: "restImmutableEntryId"
};

let res = await client.api('/me/translateExchangeIds')
    .post(convertIdResult);

```