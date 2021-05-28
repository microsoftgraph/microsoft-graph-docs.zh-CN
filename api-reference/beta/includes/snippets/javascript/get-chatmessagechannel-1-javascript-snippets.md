---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dc435fd329fb5f34934247271b6bbdc13c776cb0
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2021
ms.locfileid: "51610394"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let chatMessage = await client.api('/chats/19:8ea0e38b-efb3-4757-924a-5f94061cf8c2_97f62344-57dc-409c-88ad-c4af14158ff5@unq.gbl.spaces/messages/1612289992105')
    .version('beta')
    .get();

```