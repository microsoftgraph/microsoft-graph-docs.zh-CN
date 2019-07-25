---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1af37b5a5efcef2033955a8d17f8d79b1deb1b76
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35724343"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/ba9a3254-9f18-4209-aeb3-9e42a35b5be4')
    .version('beta')
    .delete();

```