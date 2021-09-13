---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5fdcbc51a32f903921a82a7ec56ba7b74017d77626c24b2a48801c4084ac838f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221411"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let notebook = await client.api('/me/onenote/notebooks/{id}')
    .get();

```