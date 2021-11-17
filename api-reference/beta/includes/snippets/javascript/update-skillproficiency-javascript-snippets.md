---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: da210c1e911a4faf9ea1ce5260075aa6da14d64651100ab9fc8e554352fe8544
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333317"
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