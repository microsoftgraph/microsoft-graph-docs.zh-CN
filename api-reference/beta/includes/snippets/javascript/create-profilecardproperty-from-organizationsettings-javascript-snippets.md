---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1c8f150b9f8cd0a5b08fd97e51204aa908b39873
ms.sourcegitcommit: 2c8a12389b82ee5101b2bd17eae11b42e65e52c0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2020
ms.locfileid: "45142571"
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

let res = await client.api('/organization/{organizationId}/settings/profileCardProperties')
    .version('beta')
    .post(profileCardProperties);

```