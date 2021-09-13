---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 72f877fc3560ec82330b90e5afc07edac8372b60dd7f3dd1b3fef1ef38027cdd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274097"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let filterByCurrentUser = await client.api('/identityGovernance/accessReviews/definitions/1234ea1c-8d12-457b-1234-a37dc59e54e0/instances/7070ea1c-8d12-457b-bd35-a37dc59e54e0/decisions/filterByCurrentUser(on='reviewer')')
    .get();

```