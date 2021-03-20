---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0b414b4fd71f97adf1dc04f2c21835655254b857
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941547"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let buckets = await client.api('/planner/buckets')
    .get();

```