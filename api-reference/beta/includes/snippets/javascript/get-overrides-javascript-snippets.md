---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0a4ccfb16567be6f30491bc5d34628fd910d9f7292c481571e7a8d3664d47efb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278948"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let overrides = await client.api('/me/inferenceClassification/overrides')
    .version('beta')
    .get();

```