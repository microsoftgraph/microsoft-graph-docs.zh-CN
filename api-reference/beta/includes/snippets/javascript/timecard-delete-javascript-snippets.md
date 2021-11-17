---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1b47b16cf19173b105c72d732b72b89ba7be7fe9a294a02768c6308eb1585d5c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216004"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/teams/871dbd5c-3a6a-4392-bfe1-042452793a50/schedule/timecards/3895809b-a618-4c0d-86a0-d42b25b7d74f')
    .version('beta')
    .delete();

```