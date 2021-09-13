---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b0890ed76e2748495955fa8385f01cecc8fbfa984c3d53bfe9f794cb3dbf88cd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162029"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let organizationalBranding = await client.api('/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding')
    .get();

```