---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ec5731cf658384d69a5da9d064dd7f0e5e51717
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797179"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let drive = await client.api('/drives/{driveId}')
    .version('beta')
    .get();

```