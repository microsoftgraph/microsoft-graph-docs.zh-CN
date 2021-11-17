---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7b787ca40600b67ae4cc6945ee02e53bf7178de265e665aa3d0a1469c10218cf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163944"
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