---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c360cfcb240dc7064fe98c747cc60ea0e72220bb
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2020
ms.locfileid: "41476734"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const {id} = {
  definition: [
    "definition-value"
  ],
  displayName: "displayName-value",
  isOrganizationDefault: true,
  type: "type-value"
};

let res = await client.api('/policies/tokenLifetimePolicies/{id}')
    .version('beta')
    .update({id});

```