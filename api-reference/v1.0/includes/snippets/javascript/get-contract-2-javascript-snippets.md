---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0bf82a79caa613af32c31623c3ae4f2554362aa94c7850687b28f5c5775633c2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221018"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let contracts = await client.api('/contracts')
    .get();

```