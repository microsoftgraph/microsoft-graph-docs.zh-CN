---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 735fbed28563b5255026d0f4a7b908ac68c3d48a83be57ea8c76fa3c81e9d285
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274394"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let assignmentCategories = await client.api('/education/classes/4797d052-ebf5-4018-a088-e11adc6b2cbb/assignmentCategories')
    .version('beta')
    .get();

```