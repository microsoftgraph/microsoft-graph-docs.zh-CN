---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3179256191f4c5b5edb92af3db8569a0ce5d5c29
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566642"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const profileCardProperty = {
  directoryPropertyName: "CustomAttribute1",
  annotations: [
    {
      displayName: "Cost Center",
      localizations: [
        {
          languageTag: "ru-RU",
          displayName: "центр затрат"
        }
      ]
    }
  ]
};

let res = await client.api('/organization/{organizationId}/settings/profileCardProperties')
    .version('beta')
    .post(profileCardProperty);

```