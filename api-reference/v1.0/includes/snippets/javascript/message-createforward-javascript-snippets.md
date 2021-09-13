---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e2869bfe4039c0c24c013715f98418bdd41d83768b0620a3e5b4b9d6e2279b90
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218391"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/messages/{id}/createForward')
    .post();

```