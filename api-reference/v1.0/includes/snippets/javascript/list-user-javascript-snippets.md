---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 606b69573d2902143a409f6a23aa9ee6879bbc157051d682d3816d86a390e606
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378729"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let allowedUsers = await client.api('/print/shares/{printerShareId}/allowedUsers')
    .get();

```