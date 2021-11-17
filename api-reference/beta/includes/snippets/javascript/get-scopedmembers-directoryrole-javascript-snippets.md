---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d42b8bb1a0ea04f4aa5d04e7326b9600a6a9886cce32c6c065ce145eeb6e11a6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220899"
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