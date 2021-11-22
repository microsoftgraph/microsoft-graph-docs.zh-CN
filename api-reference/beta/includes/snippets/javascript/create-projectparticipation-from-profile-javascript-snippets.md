---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5e6f6268d7969c649bd6b22189b39b74c71239ef7d39a5cca042b5ae90b53e8e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164317"
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