---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ba4763c589777e0a6f67e06811ade6ca49da3a67f33acca159623b718022e788
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219768"
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