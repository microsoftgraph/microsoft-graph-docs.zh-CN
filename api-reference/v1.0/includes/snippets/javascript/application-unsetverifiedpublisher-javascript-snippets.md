---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3f37d9d80070f45052217f1ca7fb933c761ae0d0e1737afbd0d3ba3fb19f1678
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333561"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/applications/{id}/unsetVerifiedPublisher')
    .post();

```