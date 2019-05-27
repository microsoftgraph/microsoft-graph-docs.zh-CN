---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0a685a586f58a9885b21d081f77ea1e55479e369
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34439797"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const attachment = {
    @odata.type: "#microsoft.graph.referenceAttachment",
    name: "Personal pictures",
    sourceUrl: "https://contoso.com/personal/mario_contoso_net/Documents/Pics",
    providerType: "oneDriveConsumer",
    permission: "Edit",
    isFolder: "True"
};

let res = await client.api('/me/events/AAMkAGE1M88AADUv0uAAAG=/attachments')
    .version('beta')
    .post({attachment : attachment});

```