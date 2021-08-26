---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 087595fd6e5727a8e7e1bf70dc291975d6610a9c0e03a3c98ca6c61426e130db
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333529"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/devices/{id}/registeredUsers/{id}/$ref')
    .delete();

```