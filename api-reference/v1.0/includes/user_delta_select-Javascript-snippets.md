---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 29663036263e53dd35b20c5575424959a7c665b1
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34466714"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/delta')
    .select('displayName,jobTitle,mobilePhone')
    .get();

```