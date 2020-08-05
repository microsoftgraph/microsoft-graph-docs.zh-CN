---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4dc80e6ae11e9bf9939aee180cc6a3895016585a
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46565837"
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
          languageTag: "no-NB",
          displayName: "Kostnads Senter"
        }
      ]
    }
  ]
};

let res = await client.api('/organization/{organizationId}/settings/profileCardProperties/CustomAttribute1')
    .version('beta')
    .update(profileCardProperty);

```