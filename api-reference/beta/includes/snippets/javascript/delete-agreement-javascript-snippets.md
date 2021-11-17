---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d3c6fac1a455c5450befed772715f5c5773e431ce31765bb7e870e2428d5dd90
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902550"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identityGovernance/termsOfUse/agreements/{id}')
    .version('beta')
    .delete();

```