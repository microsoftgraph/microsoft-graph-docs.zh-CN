---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 76dcc9ad32478e7dcad84dc187aa2a69e0b736a99978c8e989ad815cef5b9045
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105337"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/activities/{activity-id}/')
    .delete();

```