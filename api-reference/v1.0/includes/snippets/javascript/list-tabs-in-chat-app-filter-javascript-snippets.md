---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0acc7822d98d023c5294e3aa0203e7e0a53976a1fffe6eb9cbdda14c90167457
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904152"
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