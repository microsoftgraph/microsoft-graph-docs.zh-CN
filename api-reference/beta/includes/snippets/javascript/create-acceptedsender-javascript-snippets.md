---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7b39b3cc548629001b9e277d593d98e9915cb3820d938a1773b339fb31341c37
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274002"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  '@odata.id':'https://graph.microsoft.com/beta/users/alexd@contoso.com'
};

await client.api('/groups/{id}/acceptedSenders/$ref')
    .version('beta')
    .post(directoryObject);

```