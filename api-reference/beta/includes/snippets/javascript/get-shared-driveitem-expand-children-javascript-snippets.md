---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f005c10702e009eafbc035f3b1d2147beca143ae
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35478386"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/shares/{shareIdOrUrl}/driveItem')
    .version('beta')
    .expand('children')
    .get();

```