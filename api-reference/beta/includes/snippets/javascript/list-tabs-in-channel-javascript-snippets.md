---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 083da9b6bd3e0ef2bbd070b17c092148bf4d3df8f3133b0b08e6a6901cd45076
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106569"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tabs = await client.api('/teams/6903fa93-605b-43ef-920e-77c4729f8258/channels/19:33b76eea88574bd1969dca37e2b7a819@thread.skype/tabs')
    .version('beta')
    .expand('teamsApp')
    .get();

```