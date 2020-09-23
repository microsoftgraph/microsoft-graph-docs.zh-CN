---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cc67a821fa556609e791757a49e4a8934133ee1d
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/23/2020
ms.locfileid: "48222881"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/bitlocker/recoveryKeys/b465e4e8-e4e8-b465-e8e4-65b4e8e465b4')
    .version('beta')
    .select('key')
    .get();

```