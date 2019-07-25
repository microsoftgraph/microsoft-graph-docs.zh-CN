---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9aee84a3a1bbd8bc8e4ae2597b3f40983d4ed3cd
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35714486"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationSchool = {
  displayName: "Fabrikam Arts High School",
  description: "Magnate school for the arts. Los Angeles School District"
};

let res = await client.api('/education/schools/10002')
    .version('beta')
    .update({educationSchool : educationSchool});

```