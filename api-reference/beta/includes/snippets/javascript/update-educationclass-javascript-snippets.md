---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8f289de401a0c867feb2f90ee0cd796f724714b9
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479961"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationClass = {
  description: "History - World History 1",
  displayName: "World History Level 1",
};

let res = await client.api('/education/classes/11014')
    .version('beta')
    .update({educationClass : educationClass});

```