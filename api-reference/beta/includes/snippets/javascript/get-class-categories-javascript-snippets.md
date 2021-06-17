---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4df8c77c73cb54cb6bad6b1b600e5e16c1f103a9
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52991805"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let assignmentCategories = await client.api('/education/classes/4797d052-ebf5-4018-a088-e11adc6b2cbb/assignmentCategories')
    .version('beta')
    .get();

```