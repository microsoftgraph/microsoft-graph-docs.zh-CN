---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ee71f98d3cc0aa424ecd6d4f186a0559a2fe131
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800687"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationSchool = {
  displayName: 'Fabrikam Arts High School',
  description: 'Magnate school for the arts. Los Angeles School District'
};

await client.api('/education/schools/10002')
    .version('beta')
    .update(educationSchool);

```