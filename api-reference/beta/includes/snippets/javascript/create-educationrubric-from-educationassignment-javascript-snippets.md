---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f6cb4bf98ac06884e8d1b1aaef4fe4895ff65d8c
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636527"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationRubric = {
  @odata.id: "https://graph.microsoft.com/v1.0/education/me/rubrics/{id}"
};

let res = await client.api('/education/classes/{id}/assignments/{id}/rubric/$ref')
    .version('beta')
    .put(educationRubric);

```