---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b0db6ef4149815f211f073a2c3297518e1b76fc708c06b7b55db3e13d9d56bbd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221436"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let memberOf = await client.api('/devices/{id}/memberOf')
    .get();

```