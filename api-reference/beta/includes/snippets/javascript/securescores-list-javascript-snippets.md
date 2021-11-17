---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5365bf7ffed63a5e7cf1d7e257fe74bd218d25405868e9ad81cd736a83d74496
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333175"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let secureScores = await client.api('/security/secureScores')
    .version('beta')
    .top(1)
    .get();

```