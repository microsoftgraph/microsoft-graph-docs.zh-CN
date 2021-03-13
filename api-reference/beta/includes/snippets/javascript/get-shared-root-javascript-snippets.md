---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 46a6182099f27a9287f87674e65351055c5ae250
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802110"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sharedDriveItem = await client.api('/shares/{shareIdOrEncodedSharingUrl}')
    .version('beta')
    .get();

```