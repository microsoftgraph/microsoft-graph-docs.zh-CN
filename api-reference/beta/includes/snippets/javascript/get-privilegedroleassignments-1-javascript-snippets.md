---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 32af797d4f0f4b6df2f79c28b0bfcc8c1d9506e0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957337"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let privilegedRoleAssignments = await client.api('/privilegedRoleAssignments')
    .version('beta')
    .get();

```