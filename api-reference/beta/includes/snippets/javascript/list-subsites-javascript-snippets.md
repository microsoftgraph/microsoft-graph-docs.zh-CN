---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a5de40d46ea7a6267f91f4fb71057993364533ee
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799453"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sites = await client.api('/sites/{site-id}/sites')
    .version('beta')
    .get();

```