---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 79034253f6c8af058104b6ade9a83ed4ea6136cb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793316"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const extension = {
   '@odata.type': '#microsoft.outlookServices.openTypeExtension',
   extensionName: 'Com.Contoso.Estimate',
   companyName: 'Contoso',
   expirationDate: '2016-07-30T11:00:00.000Z',
   DealValue: 1010100,
   topPicks: [
       'Employees only',
       'Add spouse or guest',
       'Add family'
    ]
};

await client.api('/groups/37df2ff0-0de0-4c33-8aee-75289364aef6/threads/AAQkADJizZJpEWwqDHsEpV_KA==/posts/AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA=/extensions/Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate')
    .version('beta')
    .update(extension);

```