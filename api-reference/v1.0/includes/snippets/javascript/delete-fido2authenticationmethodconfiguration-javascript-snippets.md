---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b834549fb7935848129ebc97778a8056b7911af8dbf5c87f8e2698ce41f2cae9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106433"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2')
    .delete();

```