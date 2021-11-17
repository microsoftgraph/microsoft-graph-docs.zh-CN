---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fa089f0c39d781c1d60e45f424ad6ebd399b60272be53aef7e6ad2d61e0935e7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902903"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let audioRoutingGroup = await client.api('/communications/calls/{id}/audioRoutingGroups/{id}')
    .version('beta')
    .get();

```