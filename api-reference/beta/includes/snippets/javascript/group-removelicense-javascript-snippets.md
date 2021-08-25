---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d3466b5ca65cebc7abe8d11ae43599c70831274f
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58513270"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const group = {
  addLicenses: [],
  removeLicenses: [
    'c7df2760-2c81-4ef7-b578-5b5392b571df',
    'b05e124f-c7cc-45a0-a6aa-8cf78c946968'
  ]
};

await client.api('/groups/1132b215-826f-42a9-8cfe-1643d19d17fd/assignLicense')
    .version('beta')
    .post(group);

```