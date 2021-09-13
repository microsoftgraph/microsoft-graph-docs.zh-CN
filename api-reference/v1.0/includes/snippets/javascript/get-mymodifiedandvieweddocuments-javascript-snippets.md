---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fbaea3af01ca2d533563d23f21a78d9930a7f2af6ebb91301c806423f8467219
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904307"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let used = await client.api('/me/insights/used')
    .orderby('LastUsed/LastAccessedDateTime desc')
    .get();

```