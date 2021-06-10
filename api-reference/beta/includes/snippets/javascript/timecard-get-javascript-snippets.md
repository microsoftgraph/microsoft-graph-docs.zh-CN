---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 899087cfd68bd476c1edb7acac5a55f91dce27ed
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869517"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let timeCard = await client.api('/teams/fd15cad8-80f6-484f-9666-3caf695fbf32/schedule/timeCards/TCK_cc09588d-d9d2-4fa0-85dc-2aa5ef983972')
    .version('beta')
    .get();

```