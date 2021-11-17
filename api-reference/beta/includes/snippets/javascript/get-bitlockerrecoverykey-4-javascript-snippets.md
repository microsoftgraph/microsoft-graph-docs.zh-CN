---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eda51a4735ee469907afd237fa40d49f324d283f1544338363ef60e36aa4945d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105861"
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