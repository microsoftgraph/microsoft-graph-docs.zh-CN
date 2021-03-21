---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2de5d7de1d6321d9eb8e9f7f0e1ad2c846d4a7bf
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960578"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roleAssignments = await client.api('/roleManagement/deviceManagement/roleAssignments')
    .version('beta')
    .get();

```