---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b1efb1e74ce9aa7e5c3f88ca6a79490877e6f4d3
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441664"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/teams/ece6f0a1-7ca4-498b-be79-edf6c8fc4d82/channels/19:56eb04e133944cf69e603c5dac2d292e@thread.skype/members')
    .post();

```