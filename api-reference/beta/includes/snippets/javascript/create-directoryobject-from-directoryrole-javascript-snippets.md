---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: baae32d72e157d4c98dec8bc213f2a15eaba26d7
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2020
ms.locfileid: "46872673"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
    @odata.id:"https://graph.microsoft.com/beta/directoryObjects/2c891f12-928d-4da2-8d83-7d2434a0d8dc"
};

let res = await client.api('/directoryRoles/0afed502-2456-4fd4-988e-3c21924c28a7/members/$ref')
    .version('beta')
    .post(directoryObject);

```