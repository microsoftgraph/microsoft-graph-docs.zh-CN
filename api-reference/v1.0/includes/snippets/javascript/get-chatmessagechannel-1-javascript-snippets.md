---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d1d618f1cd1f1f627df5654b896035de45f8bd63
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2021
ms.locfileid: "51611650"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let chatMessage = await client.api('/chats/19:8ea0e38b-efb3-4757-924a-5f94061cf8c2_97f62344-57dc-409c-88ad-c4af14158ff5@unq.gbl.spaces/messages/1612289992105')
    .get();

```