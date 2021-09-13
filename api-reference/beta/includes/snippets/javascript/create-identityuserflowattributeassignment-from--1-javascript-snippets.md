---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a6cfb5a43b70a6c06ed16274a994bc4f7a4aa4bb2cde3c915b0daccc45829702
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215911"
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