---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dace92280bd88ccf2316200363d1d131736f493b889af386d7f0e0eeb65a3c06
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105507"
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
        content: 'clock in notes'
    }
};

await client.api('/teams/fd15cad8-80f6-484f-9666-3caf695fbf32/schedule/timeCards/clockin')
    .version('beta')
    .post(timeCard);

```