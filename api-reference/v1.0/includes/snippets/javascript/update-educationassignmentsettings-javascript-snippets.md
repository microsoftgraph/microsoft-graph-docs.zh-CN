---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ecd94c8a6771b3a5b192172fa2eaa2dfc63045fe1046c5120b093078edc1d196
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277535"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationAssignmentSettings = {
  submissionAnimationDisabled: true
};

await client.api('/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignmentSettings')
    .update(educationAssignmentSettings);

```