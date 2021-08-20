---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 89eeaa5ea891008fff51d8fd0f4e0b5e92b0a36e00ea8bd920a189be0e696ba2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409132"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let chatMessage = await client.api('/chats/19:8ea0e38b-efb3-4757-924a-5f94061cf8c2_97f62344-57dc-409c-88ad-c4af14158ff5@unq.gbl.spaces/messages/1612289992105')
    .get();

```