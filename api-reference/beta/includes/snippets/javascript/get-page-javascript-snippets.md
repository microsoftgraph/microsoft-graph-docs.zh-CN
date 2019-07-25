---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2aaa1aabc060a947a5a805dc6505f800161ed5ed
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35717505"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{site-id}/pages/{page-id}')
    .version('beta')
    .get();

```