---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9bb947fd3c07efffe7bbe25e68ace2b12b82e423
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35714446"
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