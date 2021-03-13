---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4bcf828a07dc8330f00f81a9e9a4474f36ff9d52
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791190"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/organization/{id}/certificateBasedAuthConfiguration/{id}')
    .version('beta')
    .delete();

```