---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ccfb2d7658af5f8584caa84ee814fb4826594d4
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/05/2020
ms.locfileid: "41774277"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directoryRoles/{id}/members')
    .version('beta')
    .get();

```