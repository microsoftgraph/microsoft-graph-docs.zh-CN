---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 821890cb218a479c6e739f542d1b7d39f355cbed
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955704"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let plans = await client.api('/me/planner/plans')
    .version('beta')
    .get();

```