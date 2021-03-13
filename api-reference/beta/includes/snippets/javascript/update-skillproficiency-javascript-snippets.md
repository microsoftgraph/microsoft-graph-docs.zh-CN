---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ae25dd12e088ea44ebe9c5756fb4eabd861523a0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795822"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const skillProficiency = {
  categories: [
    'Professional'
  ],
  proficiency: 'advancedProfessional'
};

await client.api('/me/profile/skills/{id}')
    .version('beta')
    .update(skillProficiency);

```