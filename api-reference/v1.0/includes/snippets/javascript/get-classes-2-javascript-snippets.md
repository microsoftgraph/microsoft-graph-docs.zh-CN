---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5f1102f044ac748bc6f926cce4edb8cb340fe27198231b16cdf06ed395b96bf4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104985"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let classes = await client.api('/education/schools/{school-id}/classes')
    .get();

```