---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1aabb926c22ae7e79071558291ee52e73405907b
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210257"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let teamworkTag = await client.api('/teams/53c53217-fe77-4383-bc5a-ed4937a1aecd/tags/MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM3ZDg4M2Q4Yi1hMTc5LTRkZDctOTNiMy1hOGQzZGUxYTIxMmUjI3RhY29VSjN2RGk==')
    .version('beta')
    .get();

```