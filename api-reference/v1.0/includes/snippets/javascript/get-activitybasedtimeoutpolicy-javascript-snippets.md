---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1d91b937b200fee3e2e644d77c23fca1c5146a1a42701a3a29c74ee7508ced71
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333364"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let activityBasedTimeoutPolicy = await client.api('/policies/activityBasedTimeoutPolicies/{id}')
    .get();

```