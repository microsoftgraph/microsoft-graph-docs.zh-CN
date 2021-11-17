---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0e2cdaf912f8678a1679379ed44b1d263b60cf1e8e2a7838ee6c8c6227b7da7c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903032"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/teams/{teamId}/schedule/timesOff/{timeOffId}')
    .version('beta')
    .delete();

```