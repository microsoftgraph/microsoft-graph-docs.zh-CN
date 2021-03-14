---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6f2e1e45c09f99ee61404de7b0389127b7437749
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795107"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/activities/{activity-id}/')
    .delete();

```