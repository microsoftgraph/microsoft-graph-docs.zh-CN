---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 94e994aaf312328ad2cc8f8931021b1af8d059b8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792576"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const webAccount = {
  description: 'My Github contributions!',
  userId: 'innocenty.popov',
  service: {
    name: 'GitHub',
    webUrl: 'https://github.com'
  }
};

await client.api('/me/profile/webAccounts')
    .version('beta')
    .post(webAccount);

```