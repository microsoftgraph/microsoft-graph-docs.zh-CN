---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3118007743f40172f17f0d361f6795f85f1b3ab122d8ed9cea54382460efdce2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162400"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let teachers = await client.api('/education/classes/11023/teachers')
    .version('beta')
    .get();

```