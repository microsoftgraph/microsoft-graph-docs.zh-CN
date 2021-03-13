---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a30eb6cda478d01d5eb159c7932c518d25fee753
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789251"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationRubric = await client.api('/education/me/rubrics/{id}')
    .version('beta')
    .get();

```