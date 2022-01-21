---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ef1c1148912e2941b6f0195ac28aa4ee75314828
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62116622"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let baseTaskList = await client.api('/me/tasks/lists/AQMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNiYQAuAAADG6BbDxY')
    .version('beta')
    .get();

```