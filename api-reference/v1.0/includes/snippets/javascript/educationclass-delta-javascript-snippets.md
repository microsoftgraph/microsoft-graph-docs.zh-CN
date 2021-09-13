---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4fa0e60b7ef375f2ef45418518944920282c0a099d65b40a9d33b14a73d1223b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215749"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/education/classes/delta')
    .get();

```