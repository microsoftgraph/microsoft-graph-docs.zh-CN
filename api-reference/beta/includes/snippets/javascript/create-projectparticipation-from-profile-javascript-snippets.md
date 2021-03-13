---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d026828a09b5a5216826adf251e72bd1a4331541
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801870"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const projectParticipation = {
  categories: [
    'Branding'
  ],
  client: {
    displayName: 'Contoso Ltd.',
    department: 'Corporate Marketing',
    webUrl: 'https://www.contoso.com'
  },
  displayName: 'Contoso Re-branding Project',
  detail: {
    company: {
      displayName: 'Adventureworks Inc.',
      department: 'Consulting',
      webUrl: 'https://adventureworks.com'
    },
    description: 'Rebranding of Contoso Ltd.',
    jobTitle: 'Lead PM Rebranding',
    role: 'project management',
    summary: 'A 6 month project to help Contoso rebrand after they were divested from a parent organization.'
  }
};

await client.api('/me/profile/projects')
    .version('beta')
    .post(projectParticipation);

```