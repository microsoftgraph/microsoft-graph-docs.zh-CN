---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f72ef8a9d257fa1b2ad2b3dcd5c07300066bfe28
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790964"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/groups/{id}/owners/{id}/$ref')
    .delete();

```