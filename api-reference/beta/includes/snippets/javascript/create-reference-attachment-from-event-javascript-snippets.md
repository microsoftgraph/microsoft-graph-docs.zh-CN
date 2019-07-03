---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0a685a586f58a9885b21d081f77ea1e55479e369
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35499588"
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