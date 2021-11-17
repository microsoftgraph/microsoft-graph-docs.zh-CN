---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b7cacf395ae3e243e89f09ac521d74c6f07510babaeacd8e50ff87548944ac52
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221502"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const timeCard = {
    atAprovedLocation: true,
    notes: {
        contentType: 'text',
        content: 'start break smaple notes'
    }
};

await client.api('/teams/fd15cad8-80f6-484f-9666-3caf695fbf32/schedule/timeCards/TCK_cc09588d-d9d2-4fa0-85dc-2aa5ef983972/startbreak')
    .version('beta')
    .post(timeCard);

```