---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b559f94a60caaae2ff411bf86f27e174a148c69a
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920281"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const b2xIdentityUserFlow = {
    id: 'Partner',
    userFlowType: 'signUpOrSignIn',
    userFlowTypeVersion: 1
};

await client.api('/identity/b2xUserFlows')
    .post(b2xIdentityUserFlow);

```