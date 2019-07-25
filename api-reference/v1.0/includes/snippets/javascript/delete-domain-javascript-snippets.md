---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e0c692776d86b734b2d8b93083f083d22dfd047f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35733548"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/domains/contoso.com')
    .delete();

```