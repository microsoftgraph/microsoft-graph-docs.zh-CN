---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3dbd9698458ee1690a55a1535c9c84d44351c7f9
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35723008"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerPlan = {
  owner: "ebf3b108-5234-4e22-b93d-656d7dae5874",
  title: "title-value"
};

let res = await client.api('/planner/plans')
    .post({plannerPlan : plannerPlan});

```