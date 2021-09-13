---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 04e84be2b02d013449310bd9976c2d34a1979f63df44c9b4c90aabe83bdea762
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329089"
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