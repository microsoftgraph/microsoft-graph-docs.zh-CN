---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0754b932f5a806cf3a6c01f9bfc3195177a41583
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34458696"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/mailFolders/inbox/messageRules/AQAAAJ5dZp8=')
    .delete();

```