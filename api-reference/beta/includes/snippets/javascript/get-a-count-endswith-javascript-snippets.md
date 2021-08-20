---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9321576b3650d9e1eaad58626a2f4da0ca3c4b992dbb1439c1d95e3c555631a8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378587"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let users = await client.api('/users')
    .version('beta')
    .header('ConsistencyLevel','eventual')
    .filter('endswith(mail,\'a@contoso.com\')')
    .orderby('userPrincipalName')
    .get();

```