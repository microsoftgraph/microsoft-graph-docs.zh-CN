---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e9b15105d6da62987dc238008921a78529a3af434d4dd7cf43ce732b2c69676a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105574"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let children = await client.api('/drives/{drive-id}/items/{item-id}/children')
    .get();

```