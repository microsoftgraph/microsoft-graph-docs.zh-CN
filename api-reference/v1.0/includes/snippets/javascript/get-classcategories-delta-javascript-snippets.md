---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b701dd48ba766f4bced49dbfdcfd44c4966c28ff
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/22/2022
ms.locfileid: "65629410"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignmentcategories/delta')
    .get();

```