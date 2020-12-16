---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f74376e4e229179d522ff530646772b6ba3536d2
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689510"
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

let res = await client.api('/identity/b2xUserFlows/B2X_1_Partner/userAttributeAssignments')
    .version('beta')
    .post(identityUserFlowAttributeAssignment);

```