---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 646347711a6d303e26e2bed6a4c41961dcb27b9e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778962"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationRubric = {
  displayName: 'Example Credit Rubric after display name patch'
};

await client.api('/education/me/rubrics/{id}')
    .version('beta')
    .update(educationRubric);

```