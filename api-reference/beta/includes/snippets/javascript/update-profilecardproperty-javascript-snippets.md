---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f7c74eb9d61e39d3146451c0b1049e76707a7a2b76006d511accae099946f87f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105990"
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