---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bfdcdd3d404ce4b517a3b12f432fea54333e4f0c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955295"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let settings = await client.api('/me/analytics/settings')
    .version('beta')
    .get();

```