---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2636cc04f4e4b1cc00de27399fdbc1bdf5f2df87712a16c32f301518e3c872e9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221096"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let list = await client.api('/sites/{site-id}/lists/{list-title}')
    .version('beta')
    .get();

```