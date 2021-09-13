---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 107ef76677bfb9287b4271ff95d11d38a5f98d3e8804f13fab6b3d5a83b463d1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904078"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let calendarView = await client.api('/me/calendarView?startDateTime=2020-01-01T19:00:00-08:00&endDateTime=2020-01-02T19:00:00-08:00')
    .get();

```