---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 47057681ed3638dabd172ae18c156b9934a5c5ed266e41d6280fba7bba802621
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216028"
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