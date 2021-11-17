---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c0dda47963220a91dffbdf9c26f5c3f85c9f33bc052a8505ae734fb4ebad3aad
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220865"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/planner/buckets/{id}')
    .version('beta')
    .delete();

```