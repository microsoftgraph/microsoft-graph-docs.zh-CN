---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d026a836c3cc601af0338239d74efd64c6f69a7f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35499595"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const programControl = {
    controlId: "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
    controlTypeId: "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    programId: "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213"
};

let res = await client.api('/programControls')
    .version('beta')
    .post({programControl : programControl});

```