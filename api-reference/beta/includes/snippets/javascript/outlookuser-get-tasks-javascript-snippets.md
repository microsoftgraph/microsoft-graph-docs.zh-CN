---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 41bd109af277a6dcbecc4e0ef5c978f3c75d7d522d4b6010a9f32733d221518c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164322"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tasks = await client.api('/me/outlook/tasks')
    .version('beta')
    .get();

```