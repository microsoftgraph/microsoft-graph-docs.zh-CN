---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8bd9bd9e3a94ee4e83f2c88a1f84b00d5e98e506
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636717"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const extension = {
  "@odata.type" : "microsoft.graph.openTypeExtension",
  "extensionName" : "Com.Contoso.Deal",
  "companyName" : "Alpine Skis",
  "dealValue" : 1010100,
  "expirationDate" : "2015-07-03T13:04:00.000Z"
};

let res = await client.api('/groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVl17IsAAA=/extensions')
    .version('beta')
    .post(extension);

```