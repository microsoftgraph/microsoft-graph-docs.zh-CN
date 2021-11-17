---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 59df2c3beded4c119356e0d5fb3965c0017e04898e0f427ae1e4f44a3a98aad6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333421"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let updatableAsset = await client.api('/admin/windows/updates/updatableAssets/983f03cd-03cd-983f-cd03-3f98cd033f98')
    .version('beta')
    .get();

```