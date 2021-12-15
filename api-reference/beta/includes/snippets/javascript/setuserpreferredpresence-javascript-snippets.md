---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6ef8e0af5578232fff35918bf5cdcbc5fd7fe0ef
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61526091"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const setUserPreferredPresence = {
  availability: 'DoNotDisturb',
  activity: 'DoNotDisturb',
  expirationDuration: 'PT8H'
};

await client.api('/users/fa8bf3dc-eca7-46b7-bad1-db199b62afc3/presence/setUserPreferredPresence')
    .version('beta')
    .post(setUserPreferredPresence);

```