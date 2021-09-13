---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 630f07b2d1126d10619a84f77b4f22f148123e9a34de9ebbbd352a7a0fbf73b1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57334113"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let schema = await client.api('/connections/contosohr/schema')
    .get();

```