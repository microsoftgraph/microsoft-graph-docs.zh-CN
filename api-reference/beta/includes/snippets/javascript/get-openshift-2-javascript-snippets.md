---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 35585ca95ba1f8b785ebb1af6d7a24c379b38ed6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962357"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let openShifts = await client.api('/teams/{id}/schedule/openShifts')
    .version('beta')
    .get();

```