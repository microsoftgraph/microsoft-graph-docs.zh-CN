---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dd284347307d229e74ecb839c7d646b1328e398f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951527"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationUser = {
  '@odata.id':'https://graph.microsoft.com/beta/education/users/13015'
};

await client.api('/education/classes/11011/members/$ref')
    .version('beta')
    .post(educationUser);

```