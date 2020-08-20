---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 60e4dc0c775432554c13f661abe0c50f843ef9a1
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46820282"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const itemPatent = {
  description: "Calculating the intent of a user to purchase an item based on the amount of time they hover their mouse over a given pixel.",
  displayName: "Inferring User Intent through browsing behaviors",
  isPending: true,
  number: "USPTO-3954432633",
  webUrl: "https://patents.gov/3954432633"
};

let res = await client.api('/me/profile/patents')
    .version('beta')
    .post(itemPatent);

```