---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 93dce2d957a5d253431885c01a455ed1ea98974c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792298"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/applications/{id}/extensionProperties/{id}')
    .delete();

```