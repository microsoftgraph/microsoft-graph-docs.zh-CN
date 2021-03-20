---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a84a90ea533ac6744e66360d48b7d8f628b09931
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50947168"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let connector = await client.api('/onPremisesPublishingProfiles/applicationProxy/connectors/{id}')
    .version('beta')
    .get();

```