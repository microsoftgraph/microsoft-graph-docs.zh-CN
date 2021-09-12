---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 250a130b7b0952e83b0aa2b13ba37d6f8d8282d7549a8fe819096b41d58ff984
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57334091"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let secureScores = await client.api('/security/secureScores')
    .top(1)
    .get();

```