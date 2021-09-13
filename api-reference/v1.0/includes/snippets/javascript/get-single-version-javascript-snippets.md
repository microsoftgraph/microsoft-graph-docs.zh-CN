---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6226f196bb66c5d9e2260a2721f4764397cfcc138fbd864363cdcc901abb9087
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409736"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let driveItemVersion = await client.api('/me/drive/items/{item-id}/versions/{version-id}')
    .get();

```