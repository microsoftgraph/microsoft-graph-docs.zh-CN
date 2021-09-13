---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ed7d36d40cd1777df2a70aab626a13005d1e59a80f9d144fba5442ddd247db2a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105360"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let list = await client.api('/sites/{site-id}/lists/{list-title}')
    .get();

```