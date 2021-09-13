---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d243bae98ba58087cfab2ff4baae3a3db25e4e42dac5b8a1fbf82fafe55ad9ac
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105093"
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