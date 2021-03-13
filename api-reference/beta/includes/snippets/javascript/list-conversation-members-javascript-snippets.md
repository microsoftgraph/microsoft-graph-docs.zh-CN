---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1dde69eb9c49ed79502848aa2ea623a3563d7aa8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50770043"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let members = await client.api('/me/chats/19:8b081ef6-4792-4def-b2c9-c363a1bf41d5_5031bb31-22c0-4f6f-9f73-91d34ab2b32d@unq.gbl.spaces/members')
    .version('beta')
    .get();

```