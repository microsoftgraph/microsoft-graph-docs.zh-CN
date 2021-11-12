---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4b4b759e376f5fc9a32df2732da0b783e435e3991752a7e4841c36979cee1635
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277749"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let subscribedSku = await client.api('/subscribedSkus/{id}')
    .version('beta')
    .get();

```