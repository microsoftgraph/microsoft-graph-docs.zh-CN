---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5a3098526d478761d1eaaa2fcc3e595c41193571
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904305"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{id}/transitiveMemberOf')
    .get();

```