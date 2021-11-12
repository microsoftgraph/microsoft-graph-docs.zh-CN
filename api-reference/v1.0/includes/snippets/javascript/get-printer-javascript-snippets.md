---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d0f117e0c85f1db85162f822cc4e35c39d1396dc8c1da52aeecbd9625ac361c7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279666"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printer = await client.api('/print/printers/{printerId}')
    .get();

```