---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c95739affabf4b7a043fa9ad2bee1ed1ae551cf4b6b3aad4a6e974a45f2779f7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105982"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let messages = await client.api('/admin/serviceAnnouncement/messages')
    .version('beta')
    .get();

```