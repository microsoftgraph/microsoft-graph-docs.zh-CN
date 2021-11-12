---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0d6cba38d1e0b0e73c650ed672895d23a03cbdbf3cd9f9851b3f1eeb763d2e47
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277219"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let directReports = await client.api('/contacts/{id}/directReports')
    .get();

```