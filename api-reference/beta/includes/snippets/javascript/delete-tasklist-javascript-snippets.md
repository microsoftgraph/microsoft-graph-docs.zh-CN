---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 39bd38fb1eb3b54f3a9e07714bfa41074f5fce26
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519286"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/tasks/lists/AAMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNiYQAu')
    .version('beta')
    .delete();

```