---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e238189ac915b8fd2f45124857a1a2bf50ca10bdfb54f53090d14246270335fd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105917"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let signIn = await client.api('/auditLogs/signIns/66ea54eb-6301-4ee5-be62-ff5a759b0100')
    .get();

```