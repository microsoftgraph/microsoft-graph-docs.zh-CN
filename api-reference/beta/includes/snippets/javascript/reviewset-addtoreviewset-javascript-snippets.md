---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f584c227d7d3b62811ddb55bc020534573f57428
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772897"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const addToReviewSet = {
    sourceCollection: {
        id: '1a9b4145d8f84e39bc45a7f68c5c5119'
    },
    additionalData: 'linkedFiles'
};

await client.api('/compliance/ediscovery/cases/080e8cad-f21f-4452-8826-0ddf7e949fdd/reviewSets/6fe25d32-8167-4625-b75c-c4181ccbd9d5/addToReviewSet')
    .version('beta')
    .post(addToReviewSet);

```