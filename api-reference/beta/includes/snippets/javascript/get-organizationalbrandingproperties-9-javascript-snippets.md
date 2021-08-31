---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3b0e8ecd60924cb79d11b9dc88e03f54461cabe33d728e0e90b695aae6e69e71
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333187"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let localizations = await client.api('/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations')
    .version('beta')
    .get();

```