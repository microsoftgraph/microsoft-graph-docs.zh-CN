---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5d5f02c4572c0664c6482555f9ae7672509260d6
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689999"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/chats/19:ea28e88c00e94c7786b065394a61f296@thread.v2/tabs/d731fca0-0f14-4537-971a-0ef9101ff13d')
    .version('beta')
    .expand('teamsApp')
    .get();

```