---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 179e04ee675db0fef1b2f77789d6a112ec30e8b6
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49946358"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityUserFlowAttributeAssignment = {
    isOptional: false,
    requiresVerification: false,
    userInputType: "TextBox",
    displayName: "Shoe size",
    userAttributeValues: [],
    userAttribute: {
        id: "extension_guid_shoeSize"
    }
};

let res = await client.api('/identity/b2cUserFlows/B2C_1_Consumer/userAttributeAssignments')
    .version('beta')
    .post(identityUserFlowAttributeAssignment);

```