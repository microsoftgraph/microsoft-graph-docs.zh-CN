---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4fb909fab4b5e8d5c7e2ed16e04c0c5948c1c41908d4f90c38b4f18839aa4af8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220555"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding')
    .delete();

```