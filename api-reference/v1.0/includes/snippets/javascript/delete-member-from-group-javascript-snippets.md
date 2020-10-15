---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a06098877ba7a939caa5ceefb7a62982cfa20a9e
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48462544"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{group-id}/members/{directory-object-id}/$ref')
    .delete();

```