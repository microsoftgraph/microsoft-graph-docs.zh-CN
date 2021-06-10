---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a4ff68a4b1d6ff0c55d60e7b24e8e312c305c6b0
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869791"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/teams/fd15cad8-80f6-484f-9666-3caf695fbf32/schedule/timeCards/TCK_cc09588d-d9d2-4fa0-85dc-2aa5ef983972/confirm')
    .version('beta')
    .post();

```