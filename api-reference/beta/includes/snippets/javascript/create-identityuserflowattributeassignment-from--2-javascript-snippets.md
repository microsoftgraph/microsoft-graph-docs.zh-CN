---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0d5ce69f07b01a89e26efe35c4cc2b3e86d7dfa38752d02bae9f86c356e29d2e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105882"
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