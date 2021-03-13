---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d71fc2ee13d4122a79037dd803a60fa565cfa11b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775337"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const team = {
  'template@odata.bind': 'https://graph.microsoft.com/beta/teamsTemplates(\'standard\')',
  displayName: 'My Sample Team',
  description: 'My Sample Team’s Description'
};

await client.api('/teams')
    .version('beta')
    .post(team);

```