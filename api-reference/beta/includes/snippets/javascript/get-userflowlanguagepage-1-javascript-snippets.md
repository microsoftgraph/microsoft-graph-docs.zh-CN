---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 43669c3bb75cb11d508e0efc10f56ff83d101e548a317fad05f00f1a7769c0c0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162688"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let defaultPages = await client.api('/identity/b2cUserFlows/B2C_1_Customer/languages/en/defaultPages')
    .version('beta')
    .get();

```