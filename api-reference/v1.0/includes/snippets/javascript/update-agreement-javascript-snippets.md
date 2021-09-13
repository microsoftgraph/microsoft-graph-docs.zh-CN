---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 640e5f0e8fd96e0489cb0344d2bd7c2f7af2e7e88374049a5789e134a5b18729
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219397"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const agreement = {
  displayName: 'Sample ToU display name',
  isViewingBeforeAcceptanceRequired: true
};

await client.api('/identityGovernance/termsOfUse/agreements/093b947f-8363-4979-a47d-4c52b33ee1be')
    .update(agreement);

```