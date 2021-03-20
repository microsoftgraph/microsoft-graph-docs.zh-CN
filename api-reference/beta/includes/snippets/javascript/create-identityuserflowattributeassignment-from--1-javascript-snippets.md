---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1c334d929bdc359c126bf7266644fa24c9959eb9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944689"
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

await client.api('/identity/b2cUserFlows/B2C_1_Consumer/userAttributeAssignments')
    .version('beta')
    .post(identityUserFlowAttributeAssignment);

```