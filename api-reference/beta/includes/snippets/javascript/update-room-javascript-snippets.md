---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 06485f8f754d6c3a8ba197bbc2070feaa7fe9739
ms.sourcegitcommit: 1138d6e84f64f3727e180da10f89b89021855c3e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2021
ms.locfileid: "50059702"
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
  capacity: 50,
  isWheelChairAccessible: false
};

let res = await client.api('/places/cf100@contoso.com')
    .version('beta')
    .update(place);

```