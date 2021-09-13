---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 810600976ee209c3726ca5baab04a9c8aed76f3f6b6bd2521501515f95f88c2b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332058"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  '@odata.id':'https://graph.microsoft.com/v1.0/users/alexd@contoso.com'
};

await client.api('/groups/{id}/acceptedSenders/$ref')
    .post(directoryObject);

```