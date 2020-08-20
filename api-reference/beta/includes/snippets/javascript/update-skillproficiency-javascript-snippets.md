---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 356d27049059e3c5e5db9cb0b262ab5add32763c
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46821036"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const skillProficiency = {
  categories: [
    "Professional"
  ],
  proficiency: "advancedProfessional"
};

let res = await client.api('/me/profile/skills/{id}')
    .version('beta')
    .update(skillProficiency);

```