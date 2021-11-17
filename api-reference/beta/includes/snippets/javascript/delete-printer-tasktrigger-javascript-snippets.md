---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bb19e55fadcd9c9d48fc0fc700a0393738115eefdca29276ac18d189fc0fc635
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105542"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/print/printers/1a5f91a7-9bd1-4d5f-bb86-f43554cac51c/taskTriggers/25be207e-1154-491f-aa68-a9f7007d4bec')
    .version('beta')
    .delete();

```