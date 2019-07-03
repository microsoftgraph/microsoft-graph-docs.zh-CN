---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 318c0d823523ae2511c6de20231478ad997c9d52
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35478972"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationUser = {
  @odata.id:"https://graph.microsoft.com/beta/education/users/14008"
};

let res = await client.api('/education/schools/{id}/users/$ref')
    .version('beta')
    .post({educationUser : educationUser});

```