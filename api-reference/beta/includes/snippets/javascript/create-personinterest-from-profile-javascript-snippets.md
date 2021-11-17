---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 03f7430401ec5093d8ad8aca3c45d73fcd671df51fb3ef6013e4e402dc4eeda5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279590"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const personInterest = {
  categories: [
    'Sports'
  ],
  description: 'World\'s greatest football club',
  displayName: 'Chelsea FC',
  webUrl: 'https://www.chelseafc.com'
};

await client.api('/me/profile/interests')
    .version('beta')
    .post(personInterest);

```