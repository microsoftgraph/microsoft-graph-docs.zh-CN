---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 248d834a1ffdf7e73b624ae5c977f535d62e8a26
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475311"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/microsoftAuthenticator')
    .version('beta')
    .delete();

```