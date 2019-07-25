---
description: 自动生成的文件。 不修改
ms.openlocfilehash: de0889463eaf7183573ac40e2e237b9aa65fe5fa
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35711918"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/rejectedSenders')
    .version('beta')
    .get();

```