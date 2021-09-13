---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 60f377bdb5043e3c4940cd5bfa3ae3c1c25aa8c984d4477de8cb2524b961dfc9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277547"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let directoryRoles = await client.api('/directoryRoles')
    .get();

```