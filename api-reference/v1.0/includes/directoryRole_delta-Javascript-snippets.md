---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2c7b229a0b437320d505aa1ed445bc6b29ae58cf
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34458167"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directoryRoles/delta')
    .get();

```