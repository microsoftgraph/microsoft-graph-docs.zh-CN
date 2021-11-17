---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 45cb452275ab9fb2de0dde614401e2857f113d894eb1212ab0e6356c7242f238
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277464"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/synchronizationProfiles/{id}')
    .version('beta')
    .delete();

```