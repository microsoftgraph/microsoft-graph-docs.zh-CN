---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 82747400f9ecc62486cf5912fe134314c93e00de
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942227"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/appCatalogs/teamsApps?requiresReview=true')
    .version('beta')
    .post();

```