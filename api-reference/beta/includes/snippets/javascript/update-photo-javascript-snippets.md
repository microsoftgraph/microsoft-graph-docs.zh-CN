---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 224cd943ec8cec4514fdfa3eea69ef438ab4b4cc
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636708"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const profilePhoto = {
  height: 99,
  width: 99,
  id: "id-value"
};

let res = await client.api('/users/{id|userPrincipalName}/photo')
    .version('beta')
    .update(profilePhoto);

```