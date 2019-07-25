---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2e93b9f9716477ed9adea2fea74e1f07f49779af
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35711002"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/applyDecisions')
    .version('beta')
    .post();

```