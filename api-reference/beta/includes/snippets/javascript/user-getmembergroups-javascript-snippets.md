---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0c6527859ba958fc1e2914e595423c624b3b81767c5ec1faf06f1021315e613e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220754"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  securityEnabledOnly: true
};

await client.api('/me/getMemberGroups')
    .version('beta')
    .post(string);

```