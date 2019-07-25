---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a3e639af0aee8cf1ce5fc456b52b29600e87d18c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35722103"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/schemaExtensions')
    .filter('id eq 'graphlearn_test'')
    .get();

```