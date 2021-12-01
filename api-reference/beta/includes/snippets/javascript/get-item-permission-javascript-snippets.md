---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f6dba69d57a53e92334538a6cbe9cb1e2fb4aa84ab317805ebe47ebb2b3f1830
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221233"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let permission = await client.api('/me/drive/items/{item-id}/permissions/{perm-id}')
    .version('beta')
    .get();

```