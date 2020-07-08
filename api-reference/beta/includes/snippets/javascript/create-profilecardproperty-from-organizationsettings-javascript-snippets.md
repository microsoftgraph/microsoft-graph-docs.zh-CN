---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c3840b4143a3d30beefff0f80f449f95451ae0f1
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2020
ms.locfileid: "45080631"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const profileCardProperties = {
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

let res = await client.api('/organization/settings/profileCardProperties')
    .version('beta')
    .post(profileCardProperties);

```