---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0929ce4801199b66f801ec67f41c00a5e7a9c69a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50465350"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062/members')
    .version('beta')
    .filter('(microsoft.graph.aadUserConversationMember/userId eq \'73761f06-2ac9-469c-9f10-279a8cc267f9\')')
    .get();

```