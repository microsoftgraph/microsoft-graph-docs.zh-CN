---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 29600d8f8bd75a9c92799a79719ff9f11d750d1d26602d5db0b1f90e0650754e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220311"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let children = await client.api('/me/drive/root/children')
    .version('beta')
    .get();

```