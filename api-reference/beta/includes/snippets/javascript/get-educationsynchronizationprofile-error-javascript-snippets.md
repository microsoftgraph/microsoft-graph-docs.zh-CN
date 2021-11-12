---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aceb937d5437b7631fd18e3ae1b0bb49a3d827736898a3f66aa5a545beebcd27
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277339"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let errors = await client.api('/education/synchronizationProfiles/{id}/errors')
    .version('beta')
    .get();

```