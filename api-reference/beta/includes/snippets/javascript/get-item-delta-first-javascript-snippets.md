---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6c403b06cb89d6daaf5d9d023820d825e46032e9
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2019
ms.locfileid: "36465015"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/root/delta')
    .version('beta')
    .get();

```