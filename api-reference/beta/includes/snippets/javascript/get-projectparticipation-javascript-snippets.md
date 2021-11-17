---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6e6ce6e9a598bf05f6339e3aad9a15b7b2fcd400190e8709bcbbc899e74405d5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161388"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let projectParticipation = await client.api('/me/profile/projects/{id}')
    .version('beta')
    .get();

```