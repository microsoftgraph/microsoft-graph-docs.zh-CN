---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9f9e78613bbd9fc6f630af55acf8cbd1a4d0d070
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35712002"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/groupLifecyclePolicies')
    .version('beta')
    .get();

```