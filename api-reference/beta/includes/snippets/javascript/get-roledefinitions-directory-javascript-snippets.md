---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9cbb303f0015f4d681bb9d20616c9e6907cb7a4ead2b2c862980ee5c7bc18b49
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106617"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roleDefinitions = await client.api('/roleManagement/directory/roleDefinitions')
    .version('beta')
    .get();

```