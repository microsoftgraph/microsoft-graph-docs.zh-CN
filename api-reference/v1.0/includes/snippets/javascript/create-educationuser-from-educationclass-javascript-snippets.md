---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4b16a9316ebbe79f009768d6aef4a59cc3b91f84
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945497"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationUser = {
  @odata.id:"https://graph.microsoft.com/v1.0/education/users/13015"
};

let res = await client.api('/education/classes/{class-id}/members/$ref')
    .post(educationUser);

```