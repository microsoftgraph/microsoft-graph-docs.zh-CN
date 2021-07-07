---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 390e6bc3500a3ab359721652ddea6981e808808d
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2021
ms.locfileid: "53316571"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let auditEvents = await client.api('/deviceManagement/virtualEndpoint/auditEvents')
    .version('beta')
    .get();

```