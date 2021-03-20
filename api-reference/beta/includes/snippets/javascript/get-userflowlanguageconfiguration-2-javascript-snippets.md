---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aaab7ed46d69122539b0930b3cdfddcdf8f3d712
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944485"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let languages = await client.api('/identity/b2xUserFlows/B2X_1_PartnerSignUp/languages')
    .version('beta')
    .get();

```