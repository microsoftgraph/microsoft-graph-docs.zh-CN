---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d63ba97ad9376231971f3dae76fa1dc57b984cf3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35478760"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const String = {
  groupIds: [
    "groupIds-value"
  ]
};

let res = await client.api('/me/checkMemberGroups')
    .version('beta')
    .post(String);

```