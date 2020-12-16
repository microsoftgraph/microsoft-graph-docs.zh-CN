---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 64cb36502e6a52be5ce18d425674ab32866b552c
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689954"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/chats/19:d65713bc498c4a428c71ef9353e6ce20@thread.v2/tabs')
    .version('beta')
    .filter('teamsApp/id eq 'com.microsoft.teamspace.tab.web'')
    .expand('teamsApp')
    .get();

```