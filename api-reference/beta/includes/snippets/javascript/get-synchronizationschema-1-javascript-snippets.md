---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7b373d82afa2d6d655fde4eaae54fbf2df7fa975c58df00e75286940c4b633fd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903041"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let synchronizationSchema = await client.api('/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema')
    .version('beta')
    .get();

```