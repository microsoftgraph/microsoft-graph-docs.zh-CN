---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8cfa0efcb4872ed7e20ab7165b96809a2cada428
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2021
ms.locfileid: "60562767"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let organizationalBranding = await client.api('/organization/84841066-274d-4ec0-a5c1-276be684bdd3/branding')
    .header('Accept-Language','0')
    .get();

```