---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 99bcfa9a5e3d160d89449d698a966e35b3333f0f223efa675b868e350c7bbad2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278235"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let members = await client.api('/chats/{id}/members')
    .get();

```