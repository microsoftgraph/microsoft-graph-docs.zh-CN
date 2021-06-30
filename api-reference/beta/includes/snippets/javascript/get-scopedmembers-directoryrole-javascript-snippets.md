---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 51edab8ef9c5362a0c398af28de8448b2d4abc3b
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207698"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let scopedMembers = await client.api('/directoryRoles/41d12a2f-caa8-4e3e-ba14-05e5102ce085/scopedMembers')
    .version('beta')
    .get();

```