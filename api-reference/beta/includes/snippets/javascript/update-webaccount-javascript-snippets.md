---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b7d88ea2e759a28c09800426da064f7e5fc8f7c99ed2b4a6f72a16d0999ade5e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220177"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const webAccount = {
  webUrl: 'https://github.com/innocenty.popov'
};

await client.api('/me/profile/webAccounts/{id}')
    .version('beta')
    .update(webAccount);

```