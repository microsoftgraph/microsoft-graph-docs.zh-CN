---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 07b394aaa1795f31c755d2bf1a93f59f70f92477
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46821318"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const languageProficiency = {
  allowedAudiences: "organization"
};

let res = await client.api('/me/profile/languages/{id}')
    .version('beta')
    .update(languageProficiency);

```