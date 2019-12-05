---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 91d42308d60436a584f9575c2f40165cbe052ade
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/05/2019
ms.locfileid: "39856719"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const updateMetadata = {
  metadata: "metadata-value",
  clientContext: "clientContext-value"
};

let res = await client.api('/communications/calls/{id}/updateMetadata')
    .version('beta')
    .post(updateMetadata);

```