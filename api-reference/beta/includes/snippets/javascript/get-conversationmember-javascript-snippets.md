---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d4f6250eee20800484291ce0183608434d508f41
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081040"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{teamsId}/members')
    .version('beta')
    .get();

```