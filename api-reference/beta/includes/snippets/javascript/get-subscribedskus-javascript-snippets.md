---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6df03ee24a5bc5a1907cc071bbbfeb3309224f8f92d3330c2f1183286750a6d4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106087"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let subscribedSkus = await client.api('/subscribedSkus')
    .version('beta')
    .get();

```