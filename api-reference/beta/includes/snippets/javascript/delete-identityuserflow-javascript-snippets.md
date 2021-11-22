---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b52ea9b6f01c143f616c6ed57a6a1748101fb669ed684edce580552c51cd5d44
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273998"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identity/userFlows/{id}')
    .version('beta')
    .delete();

```