---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 46e63c1bd65f3397424a01568c06306df4a231c2
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52239153"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let deployments = await client.api('/admin/windows/updates/deployments')
    .version('beta')
    .get();

```