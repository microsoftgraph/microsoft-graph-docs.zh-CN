---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cc78e52be98fb493bdb5732025699a07657cf9c0
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61225544"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let attributeSets = await client.api('/directory/attributeSets')
    .version('beta')
    .top(10)
    .get();

```