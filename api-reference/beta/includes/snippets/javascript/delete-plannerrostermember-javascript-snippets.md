---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2d6fa018cd2104970944910b9d9fd4b3e78c6f091c8d91f810cd46fe47313a16
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903950"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/planner/rosters/523a9d5a-f9d5-45c1-929f-b8525393515c/members/5ba84f7a-aa11-4a51-a298-9f2c7ec6bb38')
    .version('beta')
    .delete();

```