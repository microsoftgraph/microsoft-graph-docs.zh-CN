---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 915c9e58fc2e6d9c1d5ab5e04fc0f8f2e9e307d7
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44336379"
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
    .update(place);

```