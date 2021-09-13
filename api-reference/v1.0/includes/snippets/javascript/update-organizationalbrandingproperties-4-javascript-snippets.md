---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 14e91d7a1a785d9d6b677fe8293c910c23434a98ee2b5d1e93db4cf127460dad
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101323"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const organizationalBranding = {
    backgroundColor: '#FFFF33'
};

await client.api('/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding')
    .put(organizationalBranding);

```