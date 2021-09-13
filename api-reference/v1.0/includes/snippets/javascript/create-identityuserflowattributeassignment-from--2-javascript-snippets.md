---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8a7fefe8c8dd027078198480187a51c97d50346be71305a11b601cd023a05e6a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220441"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityUserFlowAttributeAssignment = {
    isOptional: false,
    requiresVerification: false,
    userInputType: 'TextBox',
    displayName: 'Shoe size',
    userAttributeValues: [],
    userAttribute: {
        id: 'extension_guid_shoeSize'
    }
};

await client.api('/identity/b2xUserFlows/B2X_1_Partner/userAttributeAssignments')
    .post(identityUserFlowAttributeAssignment);

```