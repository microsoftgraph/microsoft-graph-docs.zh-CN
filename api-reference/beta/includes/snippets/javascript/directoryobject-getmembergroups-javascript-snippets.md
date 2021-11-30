---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f2091623e65bdfce1fb6bffb231360eccd6866ab
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61226686"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
    securityEnabledOnly: false
};

await client.api('/directoryObjects/0049d944-a805-4680-9f54-3ab292090309/getMemberGroups')
    .version('beta')
    .post(string);

```