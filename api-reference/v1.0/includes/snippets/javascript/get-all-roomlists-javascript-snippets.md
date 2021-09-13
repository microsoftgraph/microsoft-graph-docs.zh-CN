---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c942dc791591acd70d29d8b4be71209603675b2c3ff8ecec2dad0d9d9f9a512b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328890"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roomlist = await client.api('/places/microsoft.graph.roomlist')
    .get();

```