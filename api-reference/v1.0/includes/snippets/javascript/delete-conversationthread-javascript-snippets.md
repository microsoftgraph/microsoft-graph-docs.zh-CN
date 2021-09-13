---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 607b2ba48c2a3e5ba4a7af041793f0d86459ca4ba070fb1f1133fba249cc69cd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332986"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/groups/{id}/threads/{id}')
    .delete();

```