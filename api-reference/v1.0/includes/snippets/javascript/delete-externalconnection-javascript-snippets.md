---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9681feded4375aca1ccde07feaa975d935bbfc18cda6be32aba41ea36fe3f80f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220425"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/connections/contosohr')
    .delete();

```