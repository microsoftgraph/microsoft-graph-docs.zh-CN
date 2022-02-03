---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 626daceca5cd971d7fddc0b51bad5593ebfdde83
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62339834"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let getCompatibleHubContentTypes = await client.api('/sites/{siteId}/lists/{listId}/contentTypes/getCompatibleHubContentTypes')
    .version('beta')
    .get();

```