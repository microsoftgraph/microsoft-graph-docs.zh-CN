---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8dbb6f2399dea4febda292b5279e382c1b3d4f27
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870673"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let timeCards = await client.api('/teams/fd15cad8-80f6-484f-9666-3caf695fbf32/schedule/timeCards')
    .version('beta')
    .filter('state eq \'clockedOut\'')
    .top(2)
    .get();

```