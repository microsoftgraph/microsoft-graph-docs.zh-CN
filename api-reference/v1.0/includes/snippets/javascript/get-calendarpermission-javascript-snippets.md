---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0de7eab56f078ba7c5d932769691b2b260be7aa91986a202306015a9e3709f8b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278853"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let calendarPermission = await client.api('/users/{id}/calendar/calendarPermissions/{id}')
    .get();

```