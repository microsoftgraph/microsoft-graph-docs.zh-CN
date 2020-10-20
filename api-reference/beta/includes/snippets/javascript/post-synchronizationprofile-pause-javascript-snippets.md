---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9bb947fd3c07efffe7bbe25e68ace2b12b82e423
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48610222"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/synchronizationProfiles/{id}/pause')
    .version('beta')
    .post();

```