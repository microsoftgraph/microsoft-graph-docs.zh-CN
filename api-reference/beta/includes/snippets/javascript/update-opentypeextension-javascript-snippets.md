---
description: 自动生成的文件。 不修改
ms.openlocfilehash: dc7a143fa4ecf48e06ce9e9fbbe25d244c874524
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35721129"
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
    .update({extension : extension});

```