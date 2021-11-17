---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9d2c2480d4ac336e461f4255153efd6e796675876021a14fdc642683ff3ff511
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902446"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let call = await client.api('/communications/calls/{id}')
    .version('beta')
    .get();

```