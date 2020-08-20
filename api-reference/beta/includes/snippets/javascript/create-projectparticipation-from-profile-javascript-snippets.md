---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5388c4e5aaa2b364ad8f49d2fe90201a1667b5d0
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46821254"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const projectParticipation = {
  categories: [
    "Branding"
  ],
  client: {
    displayName: "Contoso Ltd.",
    department: "Corporate Marketing",
    webUrl: "https://www.contoso.com"
  },
  displayName: "Contoso Re-branding Project",
  detail: {
    company: {
      displayName: "Adventureworks Inc.",
      department: "Consulting",
      webUrl: "https://adventureworks.com"
    },
    description: "Rebranding of Contoso Ltd.",
    jobTitle: "Lead PM Rebranding",
    role: "project management",
    summary: "A 6 month project to help Contoso rebrand after they were divested from a parent organization."
  }
};

let res = await client.api('/me/profile/projects')
    .version('beta')
    .post(projectParticipation);

```