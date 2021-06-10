---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3f5b3616a9f33912da305e7078e854122c3a7a91
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869012"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roleAssignments = await client.api('/roleManagement/cloudPC/roleAssignments')
    .version('beta')
    .get();

```