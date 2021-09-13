---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 308df554a5da42f693f5359e86c2e2af99a51710dc5ea486a68a841706e8a20d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903238"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const team = {
  'template@odata.bind': 'https://graph.microsoft.com/v1.0/teamsTemplates(\'standard\')',
  'group@odata.bind': 'https://graph.microsoft.com/v1.0/groups(\'71392b2f-1765-406e-86af-5907d9bdb2ab\')'
};

await client.api('/teams')
    .post(team);

```