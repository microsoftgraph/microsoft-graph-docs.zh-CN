---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 802973bef0902bd621ad35dd008a0ede098ed4f5c9339b7e51a926fb4536de8b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333623"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let calendarGroups = await client.api('/me/calendarGroups')
    .version('beta')
    .get();

```