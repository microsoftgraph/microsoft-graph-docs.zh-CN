---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b86c91ec7303fe7a123b8cf4cac8e69277b242f0
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566245"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const reviewSet = {
  displayName: "My Reviewset 3",
};

let res = await client.api('/compliance/ediscovery/cases/6f65a8e4-c6a0-4cff-8a81-c9ab5df7290d/reviewSets')
    .version('beta')
    .post(reviewSet);

```