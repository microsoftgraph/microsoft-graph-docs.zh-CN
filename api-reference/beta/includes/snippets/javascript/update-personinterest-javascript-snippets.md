---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3e33e2d68c7e54ce701d1aa1a020018884220bc5
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46821326"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const personInterest = {
  categories: [
    "Sports"
  ]
};

let res = await client.api('/me/profile/interests/{id}')
    .version('beta')
    .update(personInterest);

```