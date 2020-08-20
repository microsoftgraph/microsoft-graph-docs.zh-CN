---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7f5815bbdd038dad94ffc4ddbe8e7f5af78f41f8
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819668"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/profile/certifications/{id}')
    .version('beta')
    .get();

```