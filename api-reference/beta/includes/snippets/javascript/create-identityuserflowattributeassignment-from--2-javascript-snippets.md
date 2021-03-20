---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8f355756c08b01d3d01e51e9054996db68635c89
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944449"
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
    .version('beta')
    .post(identityUserFlowAttributeAssignment);

```