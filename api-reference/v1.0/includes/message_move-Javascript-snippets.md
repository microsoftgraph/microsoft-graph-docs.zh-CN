---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 090d22c1d173f6a601c685b2a0133f2b58546bd9
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34461560"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const message = {
  destinationId: "deleteditems"
};

let res = await client.api('/me/messages/AAMkADhAAATs28OAAA=/move')
    .post(message);

```