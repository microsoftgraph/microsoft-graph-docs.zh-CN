---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a61a964192636c94d0cd1e338ef55fcd967f2579b5545e84cb847cd999d2da6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158680"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let calendarGroups = await client.api('/me/calendarGroups')
    .get();

```