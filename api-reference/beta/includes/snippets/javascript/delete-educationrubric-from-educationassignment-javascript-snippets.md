---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 359222e076bd458eaeb95656d4cec053ac3b73e9
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52254507"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/classes/{id}/assignments/{id}/rubric/$ref')
    .version('beta')
    .delete();

```