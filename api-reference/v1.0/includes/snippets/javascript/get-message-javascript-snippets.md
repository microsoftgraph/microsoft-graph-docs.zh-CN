---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 16e6972fb0885f6330315c90c53d37abe71709b875364d821689bede1e949273
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218776"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let message = await client.api('/me/messages/AAMkADhMGAAA=')
    .get();

```