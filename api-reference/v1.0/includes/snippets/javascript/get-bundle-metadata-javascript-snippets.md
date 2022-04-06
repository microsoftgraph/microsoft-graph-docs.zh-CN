---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 107fb7f1d266fae1af9038d0f45ea47563be6828
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63757964"
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