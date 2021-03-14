---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0e1c953b590fe69e61ec2a12b0f37e21fde5935f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797964"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  ids: [
    '80a963dd-84af-4eb8-b2a6-781e444d4fb0',
    '62e90394-69f5-4237-9190-012177145e10',
    '86a64f51-3a64-4cc6-a8c8-6b8f000c0f52',
    'ac38546e-ddf3-437a-ac5c-27a94cd7a0f1'
  ]
};

await client.api('/me/checkMemberObjects')
    .post(string);

```