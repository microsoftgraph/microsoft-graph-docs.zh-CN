---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cd4443297635cb30b39e47d2605340134f9aa265
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "65946801"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let user = await client.api('/users/4562bcc8-c436-4f95-b7c0-4f8ce89dca5e')
    .version('beta')
    .select('ext55gb1l09_msLearnCourses')
    .get();

```