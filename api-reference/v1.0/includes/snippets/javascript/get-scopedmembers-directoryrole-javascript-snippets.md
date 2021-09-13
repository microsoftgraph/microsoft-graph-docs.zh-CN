---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f56efaa2ac9d3bebc54de79f703c71695468678bf0b3f9818aca56c84e0081e7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277239"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let scopedMembers = await client.api('/directoryRoles/41d12a2f-caa8-4e3e-ba14-05e5102ce085/scopedMembers')
    .get();

```