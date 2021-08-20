---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 81a137c6826fff567e3dd900b449186425ba7957d083a3fd4eefb44275f4f946
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220085"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const setPresence = {
  sessionId: '22553876-f5ab-4529-bffb-cfe50aa89f87',
  availability: 'Available',
  activity: 'Available',
  expirationDuration: 'PT1H'
};

await client.api('/users/fa8bf3dc-eca7-46b7-bad1-db199b62afc3/presence/setPresence')
    .version('beta')
    .post(setPresence);

```