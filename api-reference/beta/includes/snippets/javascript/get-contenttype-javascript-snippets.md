---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a3eaa1613c45766c6b28a5cef9f50a0aec182faa
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50770606"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let contentType = await client.api('/sites/{site-id}/contentTypes/{contentType-id}')
    .version('beta')
    .get();

```