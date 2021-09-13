---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e7247ea12ad9f485a6a75b024ba79b6f8a70942e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59038109"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/sites/{siteId}/contentTypes/{contentTypeId}/unpublish')
    .post();

```