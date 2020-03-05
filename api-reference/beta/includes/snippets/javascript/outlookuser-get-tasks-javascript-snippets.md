---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ea34866d7c3f39de14f0d042dbea7998d5b325b4
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37637527"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/outlook/tasks')
    .version('beta')
    .get();

```