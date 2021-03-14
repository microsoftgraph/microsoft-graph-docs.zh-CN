---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4d68f4b7aa436b718e06958b829f0c9c37feee2b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792313"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const team = {
  'template@odata.bind': 'https://graph.microsoft.com/v1.0/teamsTemplates(\'educationClass\')',
  displayName: 'My Class Team',
  description: 'My Class Team’s Description'
};

await client.api('/teams')
    .post(team);

```