---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c10785e6090cc70834a9a32c10e99e7d352da1033c336e1f5568a823d9b34fa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162784"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/microsoftAuthenticator')
    .version('beta')
    .delete();

```