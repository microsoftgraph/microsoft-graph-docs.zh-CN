---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e3bfb1cf9390a7ac30100d1dd65e3d5de0229756f36afb16985e040df55907f8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904161"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let messages = await client.api('/chats/19:2da4c29f6d7041eca70b638b43d45437@thread.v2/messages')
    .top(2)
    .get();

```