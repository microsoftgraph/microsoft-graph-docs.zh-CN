---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c4e88ef35b52768a815c9e23f18acf74dc3ccaf922c7888e05cd4d7134c74980
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163761"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let installedApps = await client.api('/users/{id}/teamwork/installedApps')
    .version('beta')
    .get();

```