---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 379def2c454b4a676c37ab978a463b1b0a2e2e52
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53444994"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/policies/mobileAppManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020/includedGroups/1a9db3ab-0acf-4808-99ae-e8ed581cb2e0/$ref')
    .version('beta')
    .delete();

```