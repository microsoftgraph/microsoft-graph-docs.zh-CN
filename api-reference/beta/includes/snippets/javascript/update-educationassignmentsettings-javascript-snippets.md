---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c49919b489a20b3388f8afaa3376cce7662532cc
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2021
ms.locfileid: "50092496"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationAssignmentSettings = {
  submissionAnimationDisabled: true
};

let res = await client.api('/education/classes/{id}/assignmentSettings')
    .version('beta')
    .update(educationAssignmentSettings);

```