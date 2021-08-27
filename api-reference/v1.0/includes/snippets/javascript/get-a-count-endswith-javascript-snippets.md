---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bb121c8a11087e403c0e1c753101fb94a9074448868e29de9265928ad1ebf073
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409659"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let users = await client.api('/users')
    .header('ConsistencyLevel','eventual')
    .filter('endswith(mail,\'a@contoso.com\')')
    .orderby('userPrincipalName')
    .get();

```