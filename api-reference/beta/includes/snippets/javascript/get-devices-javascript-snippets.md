---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2e4891e305bf5f81b887b823fb0e3d4b6f725e00
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805883"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let devices = await client.api('/devices')
    .version('beta')
    .get();

```