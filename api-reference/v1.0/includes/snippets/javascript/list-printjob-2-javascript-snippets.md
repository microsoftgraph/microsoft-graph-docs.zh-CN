---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 03a19c134315e74e9a59ee10d44c0ad858bf0e663d3cc5ad5f5543c535326db0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163260"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let jobs = await client.api('/print/shares/{printerShareId}/jobs')
    .get();

```