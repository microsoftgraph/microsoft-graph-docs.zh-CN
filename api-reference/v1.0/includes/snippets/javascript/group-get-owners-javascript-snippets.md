---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f00c1f2d73464ed63a445f3fe9b7c87f0b6b7bcf5c0995d97d2569c59173f98b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57107034"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let owners = await client.api('/groups/{id}/owners')
    .get();

```