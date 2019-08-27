---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 04cf9a738a254d398cac6a243d8163bbbc0e9c33
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636514"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationRubric = {
  displayName: "Example Credit Rubric after display name patch"
};

let res = await client.api('/education/me/rubrics/{id}')
    .version('beta')
    .update(educationRubric);

```