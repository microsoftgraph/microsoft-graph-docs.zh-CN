---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a52f145f61cf21526646aa7cc1fe3d23f31ae53817c6f4d2b9c930a6974448c4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57107057"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/drives/{drive-id}/items/{item-id}/versions/{version-id}/restoreVersion')
    .post();

```