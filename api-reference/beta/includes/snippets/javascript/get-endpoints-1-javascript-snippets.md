---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e2e2a13bdbba360c0cdce67f12f2d0fc75c3dd68
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961762"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let endpoints = await client.api('/groups/{id}/endpoints')
    .version('beta')
    .get();

```