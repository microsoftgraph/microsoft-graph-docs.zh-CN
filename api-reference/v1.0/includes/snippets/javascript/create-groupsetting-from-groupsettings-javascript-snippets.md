---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 18cbef42fe72bd270fcdb2724c3ee70c0ff2c756
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35468015"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const groupSetting = {
  displayName: "displayName-value",
  templateId: "templateId-value",
  values: [
    {
      name: "name-value",
      value: "value-value"
    }
  ]
};

let res = await client.api('/groupSettings')
    .post({groupSetting : groupSetting});

```