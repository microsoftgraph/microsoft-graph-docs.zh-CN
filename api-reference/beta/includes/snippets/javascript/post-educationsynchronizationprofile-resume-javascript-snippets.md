---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ba09b907027808a91b2823c030c7cc8fec942502
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35714404"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/synchronizationProfiles/{id}/resume')
    .version('beta')
    .post();

```