---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e86b7c8a5bbcf3b1aea64bf506529dd482b0b5f2
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58368853"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let mobileDeviceManagementPolicies = await client.api('/policies/mobileDeviceManagementPolicies')
    .version('beta')
    .get();

```