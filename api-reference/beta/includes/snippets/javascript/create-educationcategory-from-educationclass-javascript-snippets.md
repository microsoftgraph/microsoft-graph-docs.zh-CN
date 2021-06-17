---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 12aee219c05e402f3678197f0eca51ea318e5c29
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992340"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationCategory = {
  displayName: 'Quizzes'
};

await client.api('/education/classes/9a5e4047-c1dc-4243-9628-580d3c64b80c/assignmentCategories')
    .version('beta')
    .post(educationCategory);

```