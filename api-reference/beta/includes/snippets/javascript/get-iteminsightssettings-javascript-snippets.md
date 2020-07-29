---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5d67008f8fc5f1d81aeedf1a4f46c3ce4bf2f43e
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509625"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/organization/{organizationId}/settings/itemInsights')
    .version('beta')
    .get();

```