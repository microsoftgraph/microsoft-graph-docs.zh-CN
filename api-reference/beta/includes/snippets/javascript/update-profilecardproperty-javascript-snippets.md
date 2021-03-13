---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 000e4355aa00f1952370fb0133d40b1e908ea376
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786069"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const profileCardProperty = {
  annotations: [
    {
      localizations: [
        {
          languageTag: 'no-NB',
          displayName: 'Kostnads Senter'
        }
      ]
    }
  ]
};

await client.api('/organization/{organizationId}/settings/profileCardProperties/CustomAttribute1')
    .version('beta')
    .update(profileCardProperty);

```