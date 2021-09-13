---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5b6fbd19472fb91dfd8c8a7b61c255d8febe532b733abe6fe7c7d9c83c38a156
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162961"
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