---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2052e2450a5082fe1154f8637be61539d4069529
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50465210"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062/members')
    .filter('(microsoft.graph.aadUserConversationMember/displayName eq \'Harry Johnson\' or microsoft.graph.aadUserConversationMember/email eq \'admin@M365x987948.OnMicrosoft.com\')')
    .get();

```