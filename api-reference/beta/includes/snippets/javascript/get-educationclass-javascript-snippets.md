---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 627d58f2e8989e0f957bfbfd3d378e0b4573fa00cebce16b728ae8a0053e9747
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332499"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationClass = await client.api('/education/classes/11023')
    .version('beta')
    .get();

```