---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 086e8bc39c5bbafef3bdc427be6d390d88982ff9aef6140795227dae626e001b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333023"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/profile/emails/{id}')
    .version('beta')
    .delete();

```