---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ac661b806b1562f68cf4fbc2c6f825189a5a11d56ad67224caa539b6b6ac116
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903916"
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