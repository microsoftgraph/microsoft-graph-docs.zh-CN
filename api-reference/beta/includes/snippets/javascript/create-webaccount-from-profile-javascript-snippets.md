---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 38872d4c2e1bfbbdf52630b72a4e77cbaf519bb389c787a806a1f5139f1a0412
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163650"
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