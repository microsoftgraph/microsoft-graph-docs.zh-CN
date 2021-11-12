---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b2a42c2ac85c82e71da0a1c272bdb298cc98206eb52f3cf07bb1df34c21b7bb9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378725"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const group = {
  '@odata.id': 'https://graph.microsoft.com/v1.0/groups/{groupId}'
};

await client.api('/print/shares/{printerShareId}/allowedGroups/$ref')
    .post(group);

```