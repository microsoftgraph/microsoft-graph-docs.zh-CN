---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6072226393fe530943722dc630adf0a4fba5c549
ms.sourcegitcommit: 7dcd32f9e959bea2dfd81d9e0d4092f93da43cb7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2020
ms.locfileid: "46658067"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getM365AppUserDetail(period='D7')/content')
    .version('beta')
    .get();

```