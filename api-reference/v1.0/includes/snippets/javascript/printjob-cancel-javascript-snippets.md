---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f1722ef0e13d1c5919cfc5249b7788f15c0d583c137e9ee13a58cce8488ec5d7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162553"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/print/printers/{printerId}/jobs/{printJobId}/cancel')
    .post();

```