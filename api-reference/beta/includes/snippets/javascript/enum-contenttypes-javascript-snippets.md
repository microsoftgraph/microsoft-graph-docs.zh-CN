---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d644b3e678397721c0ea7e3c9307adfb97b497552f640599062c4f15c1576907
ms.sourcegitcommit: 24d0ea8e2bcb54c2f397133460c3d26fb0ba705f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/11/2021
ms.locfileid: "60729995"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let contentTypes = await client.api('/sites/{site-id}/lists/{list-id}/contentTypes')
    .version('beta')
    .get();

```