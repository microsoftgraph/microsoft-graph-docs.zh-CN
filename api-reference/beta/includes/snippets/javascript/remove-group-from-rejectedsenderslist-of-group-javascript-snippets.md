---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5a589af90237d49dfc03f68de2aa3cf1b8fce105
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35477914"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/rejectedSenders/$ref')
    .version('beta')
    .delete();

```