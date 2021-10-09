---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bdff01d82617a2fdb13fa581a728d833a419850a16c7225f4bb4a547b9094f14
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104551"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const application = {
  displayName: 'New display name'
};

await client.api('/applications/{id}')
    .version('beta')
    .update(application);

```