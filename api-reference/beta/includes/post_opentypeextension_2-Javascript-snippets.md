---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8f08c7eaf3975db5ad9524c1cae379f20de358e0
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34443430"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const extension = {
  "@odata.type" : "microsoft.graph.openTypeExtension",
  "extensionName" : "Com.Contoso.Referral",
  "companyName" : "Wingtip Toys",
  "dealValue" : 500050,
  "expirationDate" : "2015-12-03T10:00:00.000Z"
};

let res = await client.api('/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions')
    .version('beta')
    .post({extension : extension});

```