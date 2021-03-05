---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 744f1a8af8409bf44691328dc140618dc692048a
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475315"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/microsoftAuthenticator')
    .version('beta')
    .get();

```