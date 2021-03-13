---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 107fb7f1d266fae1af9038d0f45ea47563be6828
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788913"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let driveItem = await client.api('/drive/bundles/{bundle-id}')
    .version('beta')
    .get();

```