---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b1280db4e31de1ca880c838f92dbb511deff72e38cca5b4347a5e6c8f8ca0c38
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904294"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let claimsMappingPolicies = await client.api('/servicePrincipals/{id}/claimsMappingPolicies')
    .get();

```