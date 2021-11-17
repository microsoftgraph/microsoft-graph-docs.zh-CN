---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d6198f0f108d6b4305466a154d50f284a32e2c4e9479d0d7fc584662fc087b8e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273972"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/planner/rosters/5ba84f7a-aa11-4a51-a298-9f2c7ec6bb38')
    .version('beta')
    .delete();

```