---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ba146b9dac61e602ea5209893f429d24f9d05268
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2020
ms.locfileid: "41475744"
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

let res = await client.api('/policies/homeRealmDiscoveryPolicies/{id}')
    .version('beta')
    .update({id});

```