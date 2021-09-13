---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f67bf248d863bbbefd19dc0b4165ae188a84c1831b30daf0fc3d6529627d5bef
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278597"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/me/contactFolders/delta')
    .header('Prefer','odata.maxpagesize=2')
    .get();

```