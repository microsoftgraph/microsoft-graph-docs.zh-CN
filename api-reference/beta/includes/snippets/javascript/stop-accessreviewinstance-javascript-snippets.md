---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 34fb1c57ca7f8002d5542f7e2103b78fa582a4069b1f5acc817e1fa071cc6178
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104134"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identityGovernance/accessReviews/definitions/2b83cc42-09db-46f6-8c6e-16fec466a82d/instances/61a617dd-238f-4037-8fa5-d800e515f5bc/stop')
    .version('beta')
    .post();

```