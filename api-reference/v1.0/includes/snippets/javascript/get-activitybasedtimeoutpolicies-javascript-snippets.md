---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 415791c48e46d76326ae7d5d196deb9094db6a845d81a812b52e8d6a72417b37
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332817"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let activityBasedTimeoutPolicies = await client.api('/policies/activityBasedTimeoutPolicies')
    .get();

```