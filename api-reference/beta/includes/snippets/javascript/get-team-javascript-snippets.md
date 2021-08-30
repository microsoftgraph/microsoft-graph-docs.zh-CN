---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7348531ef994f0cdaea85af085299b2a7105a64587770e16b712568189719551
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333078"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let team = await client.api('/teams/893075dd-2487-4122-925f-022c42e20265')
    .version('beta')
    .get();

```