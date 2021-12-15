---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: edcf63127eddf8bdb5f393f8f472f1d2ea410f15
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525418"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let aQMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNiYQAuAAADG6BbDxY = await client.api('/me/tasks/lists/AQMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNiYQAuAAADG6BbDxY')
    .version('beta')
    .get();

```