---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5f5145c7a538ae318b878dc58556b81fceb56b5aa313e686814cf35e85688b63
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219019"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let messages = await client.api('/me/mailFolders/AAMkAGVmMDEzM/messages')
    .version('beta')
    .get();

```