---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 13db9daf3d6273718ba301ab059666b5b6b82f47
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081133"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{teamsId}/members')
    .version('beta')
    .delete();

```