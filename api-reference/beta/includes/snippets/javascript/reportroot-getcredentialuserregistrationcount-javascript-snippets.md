---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 90d096495e8d64cc8db48fff93521c27c63ed506e9c44f4719215e28b98cfa7a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158487"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let getCredentialUserRegistrationCount = await client.api('/reports/getCredentialUserRegistrationCount')
    .version('beta')
    .get();

```