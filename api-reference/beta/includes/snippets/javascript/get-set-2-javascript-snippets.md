---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aa5a02b3faf562bdf24d92640151f28621f2221336da82544be45ef541477889
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277979"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let set = await client.api('/termStore/sets/8ed8c9ea-7052-4c1d-a4d7-b9c10bffea6f')
    .version('beta')
    .get();

```