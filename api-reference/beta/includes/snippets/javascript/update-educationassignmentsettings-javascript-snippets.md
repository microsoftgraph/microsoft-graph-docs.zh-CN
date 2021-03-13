---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f3a0c5e5e17e4126c206a66e55f913ba862c31ae
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786521"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationAssignmentSettings = {
  submissionAnimationDisabled: true
};

await client.api('/education/classes/{id}/assignmentSettings')
    .version('beta')
    .update(educationAssignmentSettings);

```