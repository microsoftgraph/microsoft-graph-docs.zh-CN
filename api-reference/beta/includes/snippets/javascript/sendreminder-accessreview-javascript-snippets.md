---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f4b3dae19d10a1e68287fc07fef0e4ce09477afa
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48608328"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/sendReminder')
    .version('beta')
    .post();

```