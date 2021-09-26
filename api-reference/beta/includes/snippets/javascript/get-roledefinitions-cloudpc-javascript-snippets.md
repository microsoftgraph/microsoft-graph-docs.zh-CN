---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c84bfb9cc3728be5b2e5e8ed1e19020db3c1442c6a4fa7e64548439e6144d492
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904022"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roleDefinitions = await client.api('/roleManagement/cloudPC/roleDefinitions')
    .version('beta')
    .get();

```