---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7de7d893bbd67ee9622a1af8aacae1277c52e88a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802257"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let messageRules = await client.api('/me/mailFolders/inbox/messagerules')
    .version('beta')
    .get();

```