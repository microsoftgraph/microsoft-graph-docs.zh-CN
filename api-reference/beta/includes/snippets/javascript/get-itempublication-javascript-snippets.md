---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7e3b3f18f0d48273de85d7bb9f3966db4338842d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806931"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let itemPublication = await client.api('/me/profile/publications/{id}')
    .version('beta')
    .get();

```