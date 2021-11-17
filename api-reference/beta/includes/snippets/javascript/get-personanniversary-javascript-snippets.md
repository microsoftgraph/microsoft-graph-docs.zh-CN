---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 56d23fce1b9ac61e9cc0c5799c6c225d0324baaa99d74f12783eab6124da2e8d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215792"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let personAnnualEvent = await client.api('/me/profile/anniversaries/{id}')
    .version('beta')
    .get();

```