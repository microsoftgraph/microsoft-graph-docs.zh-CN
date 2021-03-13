---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0a2a8a9a652699becb038e7e5530f3208fc7a9f2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775834"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let teamsTab = await client.api('/chats/19:ea28e88c00e94c7786b065394a61f296@thread.v2/tabs/d731fca0-0f14-4537-971a-0ef9101ff13d')
    .version('beta')
    .expand('teamsApp')
    .get();

```