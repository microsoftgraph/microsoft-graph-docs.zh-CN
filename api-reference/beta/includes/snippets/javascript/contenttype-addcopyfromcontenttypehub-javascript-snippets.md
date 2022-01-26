---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ca56cb6044272465fe4b391e9a7bf223cbb4d48d
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2022
ms.locfileid: "62224746"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const contentType = {
  contentTypeId: 'String'
};

await client.api('/sites/{siteId}/lists/{listId}/contentTypes/addCopyFromContentTypeHub')
    .version('beta')
    .post(contentType);

```