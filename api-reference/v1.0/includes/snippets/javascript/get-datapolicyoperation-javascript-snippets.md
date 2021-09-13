---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a6816a01b7d4910f00d444cf6ece8a2ef9e989dae5fde982f5708eab60b0ba1e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333531"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let dataPolicyOperation = await client.api('/dataPolicyOperations/{id}')
    .get();

```