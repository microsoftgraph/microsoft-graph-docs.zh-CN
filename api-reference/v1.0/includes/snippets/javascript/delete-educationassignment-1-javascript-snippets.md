---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fcb4e549b00878274c7f0023b50089311b5c83cd1d0e8bc1015f8e6d0851a035
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57107050"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/classes/c42f493f-42b4-4e7d-8148-af894cbc518b/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8')
    .delete();

```