---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 32bfb3b45e81ca685aad07c97b7ddbf61c60378e865bf3399e1d86d317bf61de
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162049"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  '@odata.id':'https://graph.microsoft.com/beta/users/alexd@contoso.com'
};

await client.api('/groups/{id}/rejectedSenders/$ref')
    .version('beta')
    .post(directoryObject);

```