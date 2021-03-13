---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b6e5d56d1a0e7a777b04fc3205b5acbe5e18cb45
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50810227"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let driveItem = await client.api('/me/drive/root')
    .version('beta')
    .get();

```