---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 27454fe0acf18137feaefeec8fde61a15228ce80fa7e19898e72002ec92b48ac
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103774"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let secureScore = await client.api('/security/secureScores/{id}')
    .get();

```