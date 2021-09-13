---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aaaf2be1524e087dbacb6a831d178565aadb5ff1da35786b5cca425168f39200
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409793"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let call = await client.api('/communications/calls/{id}')
    .get();

```