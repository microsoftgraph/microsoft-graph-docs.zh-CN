---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: de4343e9d3173edbed9ad2ea1083ce98fa462ced
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772434"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let getApplicableContentTypesForList = await client.api('/sites/{siteId}/getApplicableContentTypesForList(listId='listId')')
    .version('beta')
    .get();

```