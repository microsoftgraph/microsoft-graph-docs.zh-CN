---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cdca44b47907200494fb9dff40e494aef68f3850
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46820032"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{userId}/profile/emails/{id}')
    .version('beta')
    .get();

```