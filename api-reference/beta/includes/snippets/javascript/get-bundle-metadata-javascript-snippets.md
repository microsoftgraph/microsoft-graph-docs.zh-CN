---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4370fb19f0f81bb3333c98db4f24d0dbb4a02489c7326a0b4fb57c81b9af3cf7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903706"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let driveItem = await client.api('/drive/bundles/{bundle-id}')
    .version('beta')
    .get();

```