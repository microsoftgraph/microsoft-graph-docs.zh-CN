---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8fdffcea271f5e938f8923d36c9eaf53924fdca9be6eddc2d1003ccb55cce1fe
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903243"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const team = {
  'template@odata.bind': 'https://graph.microsoft.com/v1.0/teamsTemplates(\'standard\')',
  displayName: 'My Sample Team',
  description: 'My Sample Team’s Description'
};

await client.api('/teams')
    .post(team);

```