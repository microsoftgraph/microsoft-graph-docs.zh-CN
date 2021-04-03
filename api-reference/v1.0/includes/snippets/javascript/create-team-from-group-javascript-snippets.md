---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: de26a5d942a0f9dac970fb34b34cb393e4a2ca98
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51509275"
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