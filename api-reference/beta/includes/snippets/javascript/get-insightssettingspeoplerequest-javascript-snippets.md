---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fd9724cd445c696af86e247255194c978e423eb5
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61346012"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let insightsSettings = await client.api('/organization/{organizationId}/settings/peopleInsights')
    .version('beta')
    .get();

```