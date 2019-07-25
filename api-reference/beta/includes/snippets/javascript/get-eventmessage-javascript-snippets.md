---
description: 自动生成的文件。 不修改
ms.openlocfilehash: efe03e7d495070275d9c085319cf3af5358c6e3b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35712365"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/AAMkADYAAAImV_lAAA=')
    .version('beta')
    .get();

```