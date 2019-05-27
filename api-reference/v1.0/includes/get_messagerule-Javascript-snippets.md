---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ff985df9e0675858063493672c3091e4530eebf9
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34477703"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/mailFolders/inbox/messageRules/AQAAAJ5dZqA=')
    .get();

```