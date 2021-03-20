---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fabe2ce8e2d1e5f96b105124b4d10055b0cee0d9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944365"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let bitlockerRecoveryKey = await client.api('/informationProtection/bitlocker/recoveryKeys/b465e4e8-e4e8-b465-e8e4-65b4e8e465b4')
    .version('beta')
    .select('key')
    .get();

```