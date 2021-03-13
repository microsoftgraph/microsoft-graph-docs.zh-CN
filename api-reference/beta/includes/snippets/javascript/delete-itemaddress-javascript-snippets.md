---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5421b227d90083686985d557890cc4c9470e4c91
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774700"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/users/{userId}/profile/addresses/{id}')
    .version('beta')
    .delete();

```