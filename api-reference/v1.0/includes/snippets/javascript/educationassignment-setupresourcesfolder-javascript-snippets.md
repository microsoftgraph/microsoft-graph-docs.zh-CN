---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 54ccc6803036109ced23e1875c1bc4f03c7d7336
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993171"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationAssignment = {
};

await client.api('/education/classes/d38ffdea-da93-46ac-90ba-d568c6073075/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/setUpResourcesFolder')
    .post(educationAssignment);

```