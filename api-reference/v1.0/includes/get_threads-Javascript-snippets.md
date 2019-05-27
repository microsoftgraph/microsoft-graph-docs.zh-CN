---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9e844a9d15987e49ba55b73ade54f7b6b00f6f6c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34450984"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/threads')
    .get();

```