---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4a77e03fc129f8d759eb922ba050524ccc6d96ec55fe2ad843588b8928c73e6a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57107044"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/email')
    .delete();

```