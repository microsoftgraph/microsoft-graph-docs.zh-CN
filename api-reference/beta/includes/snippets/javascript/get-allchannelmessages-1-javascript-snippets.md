---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a68c47c38f53393d657b38eabe41729d972edb28
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2021
ms.locfileid: "51610972"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let getAllMessages = await client.api('/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/getAllMessages')
    .version('beta')
    .get();

```