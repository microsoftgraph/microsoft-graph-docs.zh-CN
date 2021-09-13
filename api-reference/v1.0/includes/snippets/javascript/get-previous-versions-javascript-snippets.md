---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9dcd95427624ce6507a6ce7a164bd4aaf7e27add8d414862af9d1dd91f5779ae
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902284"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let versions = await client.api('/me/drive/items/{item-id}/versions')
    .get();

```