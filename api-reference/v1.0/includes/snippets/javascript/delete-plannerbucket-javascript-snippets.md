---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2b5468ca062048b4863876f0132138c4224e105a9af9eb8dca7065b39556ba26
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409490"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/planner/buckets/{id}')
    .delete();

```