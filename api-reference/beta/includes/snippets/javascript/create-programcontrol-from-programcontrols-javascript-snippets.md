---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0c72320aa34e6f33c017e4e21817b5d7de5a9af514a5623a5fc7013511591b6a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333328"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const programControl = {
    controlId: '7e59d237-2fb0-4e5d-b7bb-d4f9f9129213',
    controlTypeId: '6e4f3d20-c5c3-407f-9695-8460952bcc68',
    programId: '7e59d237-2fb0-4e5d-b7bb-d4f9f9129213'
};

await client.api('/programControls')
    .version('beta')
    .post(programControl);

```