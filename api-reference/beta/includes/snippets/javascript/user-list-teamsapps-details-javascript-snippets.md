---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9d7825bcefad90447f2051ba10cdacf5729d2b2b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50474984"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{id}/teamwork/installedApps')
    .version('beta')
    .expand('teamsAppDefinition($expand=bot)')
    .get();

```