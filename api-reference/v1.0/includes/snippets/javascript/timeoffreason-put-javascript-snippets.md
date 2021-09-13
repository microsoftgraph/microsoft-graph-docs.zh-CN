---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a68870d4035507e30faeda2ccea569664af4daf8d53c620bb705bcf9f6fd3bcc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903860"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const timeOffReason = {
  displayName: 'Vacation',
  iconType: 'plane',
  isActive: true
};

await client.api('/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}')
    .put(timeOffReason);

```