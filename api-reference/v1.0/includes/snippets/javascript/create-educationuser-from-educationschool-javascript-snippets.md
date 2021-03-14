---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6d027f8a9f6b2a69c3d190d06c9bf9a3fe85cdf5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793681"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationUser = {
  '@odata.id':'https://graph.microsoft.com/v1.0/education/users/14008'
};

await client.api('/education/schools/{id}/users/$ref')
    .post(educationUser);

```