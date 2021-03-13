---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b45082b9d8cff7b315cb5a2347adf9a0e14bcf7d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50810428"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const reviewSet = {
  displayName: 'My Reviewset 3',
};

await client.api('/compliance/ediscovery/cases/6f65a8e4-c6a0-4cff-8a81-c9ab5df7290d/reviewSets')
    .version('beta')
    .post(reviewSet);

```