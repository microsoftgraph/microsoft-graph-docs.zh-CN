---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 828aef0ac1e1eec757a680bba4a0c2361f22fd4ad28b0941893d40991095f0e1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162124"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let bitlockerRecoveryKey = await client.api('/informationProtection/bitlocker/recoveryKeys/b465e4e8-e4e8-b465-e8e4-65b4e8e465b4')
    .version('beta')
    .header('ocp-client-name','"My Friendly Client"')
    .header('ocp-client-version','"1.2"')
    .get();

```