---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1ee75ecc05eb65741e792c97010fa7ae6bcfba74
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782640"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const team = {
  'template@odata.bind': 'https://graph.microsoft.com/v1.0/teamsTemplates(\'standard\')',
  'group@odata.bind': 'https://graph.microsoft.com/v1.0/groups(\'groupId\')'
};

await client.api('/teams')
    .post(team);

```