---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2a13bc4eec0f0a9a811cfa82c7fdfd9e2f439a0b7537d8bf7f83ce3530159cea
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332294"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let identityProviders = await client.api('/identityProviders')
    .version('beta')
    .get();

```