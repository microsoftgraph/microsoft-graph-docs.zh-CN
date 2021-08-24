---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d018314a10eb1660d21b46299b16e9d2366abf0c16d37b6bed021018a7472295
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105911"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let signIns = await client.api('/auditLogs/signIns')
    .get();

```