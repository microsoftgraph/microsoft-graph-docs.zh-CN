---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 177f7c628820a8c85606ca422189e99f7f4bdf5833c9d22d091fba2e9d0ab9ca
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103941"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let templates = await client.api('/servicePrincipals/{id}/synchronization/templates')
    .version('beta')
    .get();

```