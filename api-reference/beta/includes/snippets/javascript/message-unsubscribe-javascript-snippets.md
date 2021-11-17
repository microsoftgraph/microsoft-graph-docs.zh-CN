---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ad0ff2b4dbea35b1711ba9d17353ebccad67a83904f35fa368ab4e421a98aca9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332221"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/messages/{id}/unsubscribe')
    .version('beta')
    .post();

```