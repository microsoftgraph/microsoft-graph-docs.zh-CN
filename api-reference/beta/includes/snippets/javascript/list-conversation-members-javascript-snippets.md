---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4eb6237110ad229d41ee95033fbb368eb58b4e72163bf90ec0ea19b6f62ac9ef
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163252"
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