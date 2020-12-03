---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 145a3e05b19267cb35af78c553aa8bfc0290d8fc
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522719"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directoryRoles/23f3b4b4-8a29-4420-8052-e4950273bbda')
    .get();

```