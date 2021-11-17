---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ab26905a9ebb74ef56365108d47b04ec176cb7c94dee9e93e98d329f80e17b64
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164021"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels/19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2/completeMigration')
    .version('beta')
    .post();

```