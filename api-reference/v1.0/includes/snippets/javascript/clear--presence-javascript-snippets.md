---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8faad03976be42740a5aa619895cb802abd37097
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58514220"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const clearPresence = {
  sessionId: '22553876-f5ab-4529-bffb-cfe50aa89f87'
};

await client.api('/users/fa8bf3dc-eca7-46b7-bad1-db199b62afc3/presence/clearPresence')
    .version('beta')
    .post(clearPresence);

```