---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ae12aadc2d3b0cb766679f4f766694d8f6be32f
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2020
ms.locfileid: "41476203"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/policies/claimsMappingPolicies/{id}')
    .version('beta')
    .get();

```