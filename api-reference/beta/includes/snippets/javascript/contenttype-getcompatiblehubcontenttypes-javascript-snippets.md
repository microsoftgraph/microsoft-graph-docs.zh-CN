---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f8d801cdb9ab21ac65633359469a2e6fbe5c0c37
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2022
ms.locfileid: "62225249"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let getCompatibleHubContentTypes = await client.api('//sites/{siteId}/lists/{listId}/contentTypes/getCompatibleHubContentTypes')
    .version('beta')
    .get();

```