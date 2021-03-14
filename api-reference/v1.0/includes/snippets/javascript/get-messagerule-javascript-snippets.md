---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ad3e4daa60a277d310fb2f0234623a03ab4cc132
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785432"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let messageRule = await client.api('/me/mailFolders/inbox/messageRules/AQAAAJ5dZqA=')
    .get();

```