---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 74d8efe099cf1a3d7f8fe5423a78577e1a7c5f68
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "35733751"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users')
    .select('displayName,givenName,postalCode')
    .get();

```