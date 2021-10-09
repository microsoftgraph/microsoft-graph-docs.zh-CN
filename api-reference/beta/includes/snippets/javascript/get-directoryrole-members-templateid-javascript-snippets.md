---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 151191a5167d78ae053efb2bb8009d7e95e4a76dc01856c9fad83a5bce07114b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221244"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let members = await client.api('/directoryRoles/roleTemplateId=4a5d8f65-41da-4de4-8968-e035b65339cf/members')
    .version('beta')
    .get();

```