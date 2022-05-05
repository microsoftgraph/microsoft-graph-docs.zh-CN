---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b2949f9b105bf812d9e9fe6209f9f72547210532
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65203700"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let associatedTeams = await client.api('/me/teamwork/associatedTeams')
    .version('beta')
    .get();

```