---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f688422c886ad4589068bd971f24f11e3942bc7b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35712535"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/classes/11021/assignments/19002/submissions/850f51b7/unsubmit')
    .version('beta')
    .post();

```