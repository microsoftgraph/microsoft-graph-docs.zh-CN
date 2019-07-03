---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 58d54e87b8ebd7e89ce601de1bc0c4882ba5c05a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35478685"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/')
    .version('beta')
    .filter('id eq 'Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')')
    .expand('extensions($filter=id%20eq%20'Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')')
    .get();

```