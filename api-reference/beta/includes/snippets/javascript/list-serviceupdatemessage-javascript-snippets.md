---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 794435fc0fdf7db52f9be8d4b168bd0bf3f09394
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208854"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let messages = await client.api('/admin/serviceAnnouncement/messages')
    .version('beta')
    .get();

```