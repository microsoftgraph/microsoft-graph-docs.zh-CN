---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: df8ded0c88c92c6ef0a7f0ba1620310f26af4fa195ccbe2ae61df74cb848b71d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278011"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let serviceHealth = await client.api('/admin/serviceAnnouncement/healthOverviews/Microsoft 365 suite')
    .version('beta')
    .get();

```