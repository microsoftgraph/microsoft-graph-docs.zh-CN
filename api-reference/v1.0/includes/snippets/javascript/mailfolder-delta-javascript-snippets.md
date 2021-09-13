---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ab7728be89fe78b711489759f2d78e6bc1fe580163ec5a2808b7ffc53efeb94
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220987"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/me/mailFolders/delta')
    .get();

```