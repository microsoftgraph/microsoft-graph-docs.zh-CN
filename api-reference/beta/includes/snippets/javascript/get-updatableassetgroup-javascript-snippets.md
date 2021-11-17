---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3d6d6d607881276620d8d8198e4b69b5b2b147d7dc07c2d25ebd4972ad191946
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220569"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let updatableAsset = await client.api('/admin/windows/updates/updatableAssets/5c55730b-730b-5c55-0b73-555c0b73555c')
    .version('beta')
    .get();

```