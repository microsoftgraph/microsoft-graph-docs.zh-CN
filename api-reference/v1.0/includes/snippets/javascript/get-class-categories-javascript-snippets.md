---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cf7d427c73a7cb7236e412a208c358e1c53bec4f
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993042"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let assignmentCategories = await client.api('/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignmentCategories')
    .get();

```