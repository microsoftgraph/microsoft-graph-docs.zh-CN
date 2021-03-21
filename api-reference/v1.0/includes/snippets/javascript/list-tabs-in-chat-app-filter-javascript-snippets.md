---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fafb1de431b0a143657a7cacd7999d1f1b4e03ea
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50954899"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tabs = await client.api('/chats/19:d65713bc498c4a428c71ef9353e6ce20@thread.v2/tabs')
    .filter('teamsApp/id eq \'com.microsoft.teamspace.tab.web\'')
    .expand('teamsApp')
    .get();

```