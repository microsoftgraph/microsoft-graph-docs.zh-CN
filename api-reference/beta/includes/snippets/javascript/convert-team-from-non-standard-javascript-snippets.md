---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5853d1526d33e3565da293a134006a79da53ac4cdbd5514fe03a87896cbe8ca2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378645"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const team = {
  'template@odata.bind': 'https://graph.microsoft.com/beta/teamsTemplates(\'educationClass\')',
  displayName: 'My Class Team',
  description: 'My Class Team’s Description'
};

await client.api('/teams')
    .version('beta')
    .post(team);

```