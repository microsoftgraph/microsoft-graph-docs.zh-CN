---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c5a9f425efbe5a16b0871c6694abc1f80fb2dd9a
ms.sourcegitcommit: 2a9b82dae63d8a998711679a379ae1fa89df80e0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/06/2021
ms.locfileid: "60214787"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let getAllMessages = await client.api('/teams/01fe12e0-e720-44fd-8854-28c66d1bee40/channels/getAllMessages')
    .filter('lastModifiedDateTime gt 2019-11-01T00:00:00Z and lastModifiedDateTime lt 2021-11-01T00:00:00Z')
    .get();

```