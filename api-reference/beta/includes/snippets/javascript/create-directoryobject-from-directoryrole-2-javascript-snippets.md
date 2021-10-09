---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cc9c8363bb5a36ace5a52434cb08ed55ba0f3f5217b18bc3ead0b467fe53cb6f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105223"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
    '@odata.id':'https://graph.microsoft.com/beta/directoryObjects/2c891f12-928d-4da2-8d83-7d2434a0d8dc'
};

await client.api('/directoryRoles/0afed502-2456-4fd4-988e-3c21924c28a7/members/$ref')
    .version('beta')
    .post(directoryObject);

```