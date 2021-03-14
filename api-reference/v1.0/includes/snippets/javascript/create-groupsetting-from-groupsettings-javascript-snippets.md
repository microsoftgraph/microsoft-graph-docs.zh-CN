---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ee2b0fcbf11c42d82943d769032e869cca9213f6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809181"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const groupSetting = {
  displayName: 'displayName-value',
  templateId: 'templateId-value',
  values: [
    {
      name: 'name-value',
      value: 'value-value'
    }
  ]
};

await client.api('/groupSettings')
    .post(groupSetting);

```