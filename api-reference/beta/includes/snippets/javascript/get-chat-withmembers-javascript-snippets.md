---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ba1ffe70000f1c48ce8f596f42fcfc48bd01da5f
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080255"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let chat = await client.api('/chats/19:b8577894a63548969c5c92bb9c80c5e1@thread.v2')
    .version('beta')
    .expand('members')
    .get();

```