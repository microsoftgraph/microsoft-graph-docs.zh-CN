---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ce71987745815b3e813adfc820010547e4655d4
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208041"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let scopedMembers = await client.api('/directoryRoles/41d12a2f-caa8-4e3e-ba14-05e5102ce085/scopedMembers')
    .get();

```