---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2fc1fb402216053df642fb6404e502e0d9c31f353e09a94f968800c00dc5b439
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277558"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tabs = await client.api('/teams/6903fa93-605b-43ef-920e-77c4729f8258/channels/19:33b76eea88574bd1969dca37e2b7a819@thread.skype/tabs')
    .filter('teamsApp/id eq \'com.microsoft.teamspace.tab.planner\'')
    .expand('teamsApp')
    .get();

```