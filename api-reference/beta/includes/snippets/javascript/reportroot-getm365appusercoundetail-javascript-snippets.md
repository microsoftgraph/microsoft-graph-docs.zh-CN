---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 092c7374365e274715a0f31c78669cb7bfc88fc4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792218"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let stream = await client.api('/reports/getM365AppUserDetail(period='D7')/content')
    .version('beta')
    .get();

```