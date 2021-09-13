---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b46a7662fbb4525f04774954216156c11e7d0c61740af2d0bd1107bf079628d6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162630"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identityGovernance/accessReviews/definitions/e6cafba0-cbf0-4748-8868-0810c7f4cc06/instances/1234fba0-cbf0-5678-8868-0810c7f91006/acceptRecommendations')
    .post();

```