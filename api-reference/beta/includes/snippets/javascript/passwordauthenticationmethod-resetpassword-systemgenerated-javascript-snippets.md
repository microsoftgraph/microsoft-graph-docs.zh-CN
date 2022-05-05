---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9bd4f04dd872a7f08071cd79b3a9f24076dfbd21
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65220317"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/users/6ea91a8d-e32e-41a1-b7bd-d2d185eed0e0/authentication/passwordMethods/28c10230-6103-485e-b985-444c60001490/resetPassword')
    .version('beta')
    .post();

```