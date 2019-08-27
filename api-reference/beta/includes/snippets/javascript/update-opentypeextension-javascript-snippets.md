---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 93f778f3940ea1a5c01340e28f75a5352dd51adc
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636668"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const extension = {
   @odata.type: "#microsoft.outlookServices.openTypeExtension",
   extensionName: "Com.Contoso.Estimate",
   companyName: "Contoso",
   expirationDate: "2016-07-30T11:00:00.000Z",
   DealValue: 1010100,
   topPicks: [
       "Employees only",
       "Add spouse or guest",
       "Add family"
    ]
};

let res = await client.api('/groups/37df2ff0-0de0-4c33-8aee-75289364aef6/threads/AAQkADJizZJpEWwqDHsEpV_KA==/posts/AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA=/extensions/Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate')
    .version('beta')
    .update(extension);

```