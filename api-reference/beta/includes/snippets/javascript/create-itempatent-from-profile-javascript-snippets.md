---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a6695260eca49e6950314a5b9caa67b843a80c95c73961b3a5c0937b3920cdf9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106287"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const itemPatent = {
  description: 'Calculating the intent of a user to purchase an item based on the amount of time they hover their mouse over a given pixel.',
  displayName: 'Inferring User Intent through browsing behaviors',
  isPending: true,
  number: 'USPTO-3954432633',
  webUrl: 'https://patents.gov/3954432633'
};

await client.api('/me/profile/patents')
    .version('beta')
    .post(itemPatent);

```