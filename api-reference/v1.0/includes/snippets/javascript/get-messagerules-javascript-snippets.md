---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2323aead66db411323ebf6530bccc714c5200c7f460d4da73b470a5c04cbf4a4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903892"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let messageRules = await client.api('/me/mailFolders/inbox/messageRules')
    .get();

```