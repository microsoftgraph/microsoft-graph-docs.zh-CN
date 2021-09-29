---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: db66679e574b42fe98a3ee273bff8465e76fe13f
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59995471"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let localizations = await client.api('/organization/84841066-274d-4ec0-a5c1-276be684bdd3/branding/localizations/')
    .version('beta')
    .get();

```