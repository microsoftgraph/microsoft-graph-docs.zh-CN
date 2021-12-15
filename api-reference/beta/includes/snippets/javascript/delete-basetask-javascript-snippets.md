---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: adf1be8f390c682ca734ce7514f40d02d6e33f51
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61524544"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/tasks/lists/AAMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNiYQAu/tasks/AAkALgAAAAAAHYQDEapmEc2byACqAC-EWg0AkOO4xOT')
    .version('beta')
    .delete();

```