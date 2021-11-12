---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9452077dc7db62ac406ce68b985667210bbf0d9e48c8d686aa1a28c47dcf89b4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105741"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/me/mailFolders/{id}/messages/delta')
    .version('beta')
    .get();

```