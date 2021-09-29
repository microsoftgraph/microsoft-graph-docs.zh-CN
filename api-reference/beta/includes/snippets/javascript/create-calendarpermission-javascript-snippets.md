---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 59afaf9388c123826b8c2c9b1f0d90d62b6a3fb8
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59995685"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const calendarPermission = {
    emailAddress: {
        name: 'Samantha Booth',
        address: 'samanthab@adatum.onmicrosoft.com'
    },
    isInsideOrganization: true,
    isRemovable: true,
    role: 'read'
};

await client.api('/users/458d4c95-124e-49da-ba9d-1dd0387e682e/calendar/calendarPermissions')
    .version('beta')
    .post(calendarPermission);

```