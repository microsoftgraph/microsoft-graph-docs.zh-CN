---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 739ca6a950c9c2bad6de820c11ef341bb1ba0b242ed72c1cce503607c09a5a2f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277207"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/schemaExtensions/{id}')
    .delete();

```