---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5edd001346a32cc43bd4f729cbfb26d5516c247f
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209799"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let decisions = await client.api('/identityGovernance/accessReviews/definitions/abadf3b6-8ea4-4dea-90a5-9eac8fe93fbd/instances/7070ea1c-8d12-457b-bd35-a37dc59e54e0/decisions')
    .get();

```