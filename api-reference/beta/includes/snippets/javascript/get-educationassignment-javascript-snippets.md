---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f0a1210b9cf909684982d78a1bb740020dcd54dce6172951b1d545b03bfa20a9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220699"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationAssignment = await client.api('/education/classes/11014/assignments/19002')
    .version('beta')
    .get();

```