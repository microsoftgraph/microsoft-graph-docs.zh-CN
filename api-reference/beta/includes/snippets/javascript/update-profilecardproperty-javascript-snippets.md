---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 023d364bf3d939b22d85d891dee8717c53338364
ms.sourcegitcommit: 2c8a12389b82ee5101b2bd17eae11b42e65e52c0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2020
ms.locfileid: "45142557"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const customAttribute1 = {
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
    .update(customAttribute1);

```