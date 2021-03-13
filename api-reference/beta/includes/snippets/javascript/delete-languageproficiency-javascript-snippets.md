---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7a9f56357b31eb8a69f11e9091b6b4a07142d52a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803929"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/profile/languages/{id}')
    .version('beta')
    .delete();

```