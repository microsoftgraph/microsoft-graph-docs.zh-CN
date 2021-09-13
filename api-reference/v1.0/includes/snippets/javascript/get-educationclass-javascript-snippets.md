---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: add56944ad64c73861c3788e436edcb94217ce2f740fd48efee4aee3d082b36f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105003"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationClass = await client.api('/education/classes/{educationClassId}')
    .get();

```