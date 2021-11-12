---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2543a4adaab0d54370d32d13038f045c877b5f4723bbd7d9be0eea01a46f5808
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106368"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const teamsTab = {
  displayName: 'My Contoso Tab - updated again'
};

await client.api('/chats/19:d65713bc498c4a428c71ef9353e6ce20@thread.v2/tabs/794f0e4e-4d10-4bb5-9079-3a465a629eff')
    .version('beta')
    .update(teamsTab);

```