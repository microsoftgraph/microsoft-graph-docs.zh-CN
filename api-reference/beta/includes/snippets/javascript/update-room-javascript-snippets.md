---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 891a1e030ef78e5bc9b54b732ab0cb28bab6800c
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/15/2019
ms.locfileid: "37997039"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const place = {
  @odata.type: "microsoft.graph.room",
  nickname: "Conf Room",
  building: "1",
  label: "100",
  capacity: "50",
  isWheelchairAccessible: false
};

let res = await client.api('/places/cf100@contoso.com')
    .version('beta')
    .update(place);

```