---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7f81c346be18c934b59c6156f451cc373baf183c
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37637471"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/tasks')
    .version('beta')
    .get();

```