---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0399f6cdae4b65c616c38f87951abc5699ace652ff47d81d977b6518c6e06895
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332927"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let driveItemVersion = await client.api('/me/drive/items/{item-id}/versions/{version-id}')
    .version('beta')
    .get();

```