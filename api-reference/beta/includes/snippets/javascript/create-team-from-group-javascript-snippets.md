---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 65db8caadac4f73fe98800b4b236d90370f2082309c25034e71a977381c2fbec
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378646"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const team = {
  'template@odata.bind': 'https://graph.microsoft.com/beta/teamsTemplates(\'standard\')',
  'group@odata.bind': 'https://graph.microsoft.com/beta/groups(\'71392b2f-1765-406e-86af-5907d9bdb2ab\')'
};

await client.api('/teams')
    .version('beta')
    .post(team);

```