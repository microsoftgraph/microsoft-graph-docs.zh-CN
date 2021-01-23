---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fe4f6557c7e5aa9dc1b593896de670b7d0c651e4
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49946323"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationUser = {
  @odata.id:"https://graph.microsoft.com/beta/education/users/13015"
};

let res = await client.api('/education/classes/11011/members/$ref')
    .version('beta')
    .post(educationUser);

```