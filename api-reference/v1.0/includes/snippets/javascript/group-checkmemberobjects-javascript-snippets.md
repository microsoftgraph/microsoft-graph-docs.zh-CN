---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cf25ff0697ce3867c4045b103e5b0559f8d9df4a4d74fc106cb6711d194d2792
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333958"
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

await client.api('/groups/{id}/checkMemberObjects')
    .post(string);

```