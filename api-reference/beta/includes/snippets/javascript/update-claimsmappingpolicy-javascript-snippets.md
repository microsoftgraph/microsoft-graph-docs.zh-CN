---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 88125cdc8c26235c878718a4c86bb31bfc386150
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2020
ms.locfileid: "41476327"
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

let res = await client.api('/policies/claimsMappingPolicies/{id}')
    .version('beta')
    .update({id});

```