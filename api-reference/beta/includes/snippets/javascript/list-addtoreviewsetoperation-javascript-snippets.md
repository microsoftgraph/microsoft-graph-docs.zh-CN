---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 478f041a894af0bce23401b9f21e59ad553c2d35
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772651"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let addToReviewSetOperation = await client.api('/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/sourceCollections/1a9b4145d8f84e39bc45a7f68c5c5119/addToReviewSetOperation')
    .version('beta')
    .get();

```