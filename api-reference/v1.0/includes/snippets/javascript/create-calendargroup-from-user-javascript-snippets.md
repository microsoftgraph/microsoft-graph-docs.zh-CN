---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3d8d71588d9e9ed410cb13faddfc416830a176f655ae60ac86d166c2e81943c7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277372"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const calendarGroup = {
  name: 'Personal events'
};

await client.api('/me/calendarGroups')
    .post(calendarGroup);

```