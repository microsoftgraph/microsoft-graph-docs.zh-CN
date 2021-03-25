---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 04826345ca0bbdedbaba3e91aa1eaa001a99494e
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201791"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let members = await client.api('/me/chats/19:8b081ef6-4792-4def-b2c9-c363a1bf41d5_5031bb31-22c0-4f6f-9f73-91d34ab2b32d@unq.gbl.spaces/members')
    .get();

```