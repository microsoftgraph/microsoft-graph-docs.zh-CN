---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 75fdc55121c39e3102f17907e7576dedd0436f724d1d81ee44e9eda40f9b9c0c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220702"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationRubric = await client.api('/education/classes/{id}/assignments/{id}/rubric')
    .version('beta')
    .get();

```