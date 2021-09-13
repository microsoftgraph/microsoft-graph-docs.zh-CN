---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 135f5935bdb8d78c05e9550019713038c217ac937fabcd2984c91c683b1fc5c2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106532"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let itemPatent = await client.api('/me/profile/patents/{id}')
    .version('beta')
    .get();

```