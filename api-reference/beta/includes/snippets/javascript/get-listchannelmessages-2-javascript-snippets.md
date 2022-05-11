---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fae1aec6c82ed10c08d19c6622da60082f660d2c
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65315017"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let messages = await client.api('/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages?top=3')
    .version('beta')
    .get();

```