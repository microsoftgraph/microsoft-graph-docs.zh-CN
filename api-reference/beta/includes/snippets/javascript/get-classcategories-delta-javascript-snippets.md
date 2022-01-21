---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: be15a1701ff23c093b30168f6ab8e20cc2d9a6f0
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137746"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignmentcategories/delta')
    .version('beta')
    .get();

```