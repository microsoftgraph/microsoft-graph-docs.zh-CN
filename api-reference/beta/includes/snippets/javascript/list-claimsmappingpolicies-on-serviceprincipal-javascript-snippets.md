---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 79b6a56c56ced59f0da2382f10fbfb277429c2768abe727d0a274834dea16fb4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215777"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let claimsMappingPolicies = await client.api('/servicePrincipals/{id}/claimsMappingPolicies')
    .version('beta')
    .get();

```