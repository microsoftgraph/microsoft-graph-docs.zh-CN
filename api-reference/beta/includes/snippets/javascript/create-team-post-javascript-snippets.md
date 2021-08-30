---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a8a29422c3c64f8f9b2949b486f099b6368642c09a9c32e9a49de3313506cc5d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378653"
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