---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1a9a0da0ff31f4a6caa8e56f7b9ef6a40b6d5218
ms.sourcegitcommit: 22bd45d272681658d46a8b99af3c3eabc7b05cb1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/18/2021
ms.locfileid: "58384137"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identityGovernance/entitlementManagement/accessPackages/fb449cf8-3a59-4d86-bdfd-a1b7299681de/getApplicablePolicyRequirements')
    .version('beta')
    .post();

```