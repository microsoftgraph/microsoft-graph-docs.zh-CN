---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5553948b4cd7c90d3c0ee516690c5c5cde943c9c086f99e65dd9c30be470e788
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219897"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let synchronizationSchema = await client.api('/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema')
    .version('beta')
    .header('Authorization','Bearer {Token}')
    .get();

```