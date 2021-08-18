---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fc4d9a05b14fea31f684653bfbfbec1a99b3da25f3395a5adac94c6301697658
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163143"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationCategory = await client.api('/education/classes/dacbf757-888d-42ae-b701-5e57cec300ae/assignmentCategories/7f64924d-4cdb-4e54-8c37-c0f3d46f0747')
    .version('beta')
    .get();

```