---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 872d933b665b514defaf772ed7da9b45296605d1
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475096"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/kim@contoso.com/authentication/temporaryAccessPassMethods/{id}')
    .version('beta')
    .delete();

```