---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3c5646ffb00e272ff2f2b4adf40b90bb66bddad0
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49690832"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062/members')
    .version('beta')
    .filter('(microsoft.graph.aadUserConversationMember/userId eq '73761f06-2ac9-469c-9f10-279a8cc267f9')')
    .get();

```