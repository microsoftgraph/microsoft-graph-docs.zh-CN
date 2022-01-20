---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ab11071104a632a413be68347316db43276172d0c2f814699ef5147e3c45fc2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218869"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let functions = await client.api('/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/functions')
    .version('beta')
    .get();

```