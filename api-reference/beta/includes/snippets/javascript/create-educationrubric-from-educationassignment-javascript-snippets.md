---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d613e07fefb01a7ea31a15d0d629c9734d255967
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461140"
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
    .put({educationRubric : educationRubric});

```