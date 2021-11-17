---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4cc9c6639fdde25fec445df29d7b03d5d2281f36b4c9055019f216f4a42b2ac8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902423"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/profile/educationalActivities/{id}')
    .version('beta')
    .delete();

```