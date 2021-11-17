---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dba45623ae0551178681abe8053347634624eb0bdc0bd9da0c9abb2dfdeb39b5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106906"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/synchronizationProfiles/{id}/pause')
    .version('beta')
    .post();

```