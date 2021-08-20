---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ce00ea96cb3fd86da7a3bd043e0cedbeaac74d2929778bc5e1423d6691b1a761
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333987"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let devices = await client.api('/devices')
    .header('ConsistencyLevel','eventual')
    .search('displayName:Android')
    .get();

```