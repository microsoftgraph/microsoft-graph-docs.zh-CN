---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b73428b951beb9dff91268c4bc0d21df3249ce56
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2019
ms.locfileid: "36460959"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationRubric = {
  displayName: "Example Credit Rubric after display name patch"
};

let res = await client.api('/education/me/rubrics/{id}')
    .version('beta')
    .update({educationRubric : educationRubric});

```