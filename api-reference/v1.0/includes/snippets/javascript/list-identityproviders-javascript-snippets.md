---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7aaf37167e101c4dc12cead156e52d95c8f19b4c241cf90ef7420471084d3493
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218394"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let identityProviders = await client.api('/identityProviders')
    .get();

```