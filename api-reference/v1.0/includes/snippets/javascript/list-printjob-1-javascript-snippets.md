---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 188d304ed3c45a999be6968ece0776961b3c782f7f5c065d62acef522594f8dc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158413"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let jobs = await client.api('/print/printers/{printerId}/jobs')
    .get();

```