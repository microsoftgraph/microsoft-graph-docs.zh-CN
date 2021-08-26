---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 52ca94ab506c680602aa47bfb1548b1e94ca735be784f0a9ef8b12f45b3d556d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162195"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const message = {
  destinationId: 'destinationId-value'
};

await client.api('/me/messages/{id}/copy')
    .version('beta')
    .post(message);

```