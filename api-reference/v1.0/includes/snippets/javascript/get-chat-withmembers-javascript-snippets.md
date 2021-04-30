---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5b03b8b937d346d2494688641d8e18c707637181
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080593"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let chat = await client.api('/chats/19:b8577894a63548969c5c92bb9c80c5e1@thread.v2')
    .expand('members')
    .get();

```