---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7c577407f5b231f624aa1c754a438e7a37e62ab8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779223"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const personWebsite = {
  categories: [
    'football'
  ],
  displayName: 'Lyn Damer',
  webUrl: 'www.lyndamer.no'
};

await client.api('/me/profile/websites')
    .version('beta')
    .post(personWebsite);

```