---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9e889f9d9038299e1a373b268c2b8f55fa9c139f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809483"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let driveItem = await client.api('/shares/{shareIdOrUrl}/driveItem')
    .version('beta')
    .expand('children')
    .get();

```