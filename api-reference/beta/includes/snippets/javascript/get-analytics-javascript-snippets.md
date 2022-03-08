---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9ea7c9eb7b618af75fa6ce435e1ccf8ea8d97f459400e956883007b5f531f952
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219194"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let itemAnalytics = await client.api('/drives/{drive-id}/items/{item-id}/analytics')
    .version('beta')
    .get();

```