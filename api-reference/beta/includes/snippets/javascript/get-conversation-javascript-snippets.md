---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ea1522883151b5aab5092cbb113be8e1120cc168c0030796c3e64f0c8448376c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104830"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let conversation = await client.api('/groups/{id}/conversations/{id}')
    .version('beta')
    .get();

```