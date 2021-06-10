---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1e4fbb4cecca62a370a97be20faba2ca5412690f
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869812"
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