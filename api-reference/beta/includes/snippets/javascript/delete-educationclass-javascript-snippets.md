---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0b8573b756f7aa2f1022e03e6a79880cb4cec1a91a0cd6edc384e260cac2d496
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220298"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/classes/11022')
    .version('beta')
    .delete();

```