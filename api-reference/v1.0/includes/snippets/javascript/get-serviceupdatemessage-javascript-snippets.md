---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a10132e324a2ba61376042f7f08e298883311252
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58257996"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let serviceUpdateMessage = await client.api('/admin/serviceAnnouncement/messages/MC172851')
    .get();

```