---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f53f10fe509e8c279b4d483f38f9d93dd39b30ab
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "61021914"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let mobilityManagementPolicy = await client.api('/policies/mobileDeviceManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020')
    .version('beta')
    .get();

```