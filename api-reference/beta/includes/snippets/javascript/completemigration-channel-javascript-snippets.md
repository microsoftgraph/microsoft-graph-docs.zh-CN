---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 32a41f179e5b6aaa1a9cd61ea6a154290d74e7df
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781966"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/teams/{teamId}/channels/{channelId}/completeMigration')
    .version('beta')
    .post();

```