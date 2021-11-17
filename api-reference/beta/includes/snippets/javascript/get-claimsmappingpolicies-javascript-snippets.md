---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3c84d030ce131dee3f53c7073acf4ed8e903d909e5d8668fa8d66c1b46472319
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164010"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let claimsMappingPolicies = await client.api('/policies/claimsMappingPolicies')
    .version('beta')
    .get();

```