---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 405e12d40315f02d7e7e3ea052533b8fd507c769d4ce1b022bda29f8bbde6049
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106565"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let chat = await client.api('/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5/chats/19:8b081ef6-4792-4def-b2c9-c363a1bf41d5_877192bd-9183-47d3-a74c-8aa0426716cf@unq.gbl.spaces')
    .version('beta')
    .get();

```