---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eef007cc2bdbef579c6c58a6e3f3942072ea1e45
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470714"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const extension = {
   '@odata.type': 'Microsoft.OutlookServices.OpenTypeExtension',
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
    .update(extension);

```