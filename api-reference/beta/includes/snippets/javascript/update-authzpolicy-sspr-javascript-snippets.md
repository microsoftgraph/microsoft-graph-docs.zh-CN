---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b60d337343bfeb167db5743c38ae2e04cce164373b795938370adb38fc93050a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903185"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authorizationPolicy = {
   allowedToUseSSPR: true
};

await client.api('/policies/authorizationPolicy/authorizationPolicy')
    .version('beta')
    .update(authorizationPolicy);

```