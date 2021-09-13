---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 10a8347387a0395a8be2aff430106f924c03fd96b533c7e405d6c218dea1baad
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219656"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let stream = await client.api('/me/drive/items/{item-id}/versions/{version-id}/content')
    .get();

```