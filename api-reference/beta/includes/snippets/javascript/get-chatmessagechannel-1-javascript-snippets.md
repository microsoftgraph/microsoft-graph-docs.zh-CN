---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8d6d83a4aeff96ff693fd72318b3c2b943c12c6540bd11ba025f885cb4e91a92
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218523"
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