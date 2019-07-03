---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3060921e418909d368b80c156f1cc5e6c832ebaa
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35499887"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/drives/{driveId}')
    .version('beta')
    .get();

```