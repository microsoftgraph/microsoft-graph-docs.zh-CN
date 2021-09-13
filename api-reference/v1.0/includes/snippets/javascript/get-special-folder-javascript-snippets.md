---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3d325fd8c5f273d8e7e2fdd930bb2c308e46f2de8cbbf8ba3f216b5a11ff151a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333808"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let driveItem = await client.api('/me/drive/special/{name}')
    .get();

```