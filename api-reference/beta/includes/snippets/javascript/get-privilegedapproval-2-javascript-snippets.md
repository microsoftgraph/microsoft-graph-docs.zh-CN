---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e20e18cf8826e7a52d532c5d689eb23a50671e66
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961427"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let privilegedApproval = await client.api('/privilegedApproval')
    .version('beta')
    .get();

```