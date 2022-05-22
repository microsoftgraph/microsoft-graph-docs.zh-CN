---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ac7cfbb18be12c86d16e320ce5e220661c5781b
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/22/2022
ms.locfileid: "65628955"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/teams/ece6f0a1-7ca4-498b-be79-edf6c8fc4d82/channels/19:56eb04e133944cf69e603c5dac2d292e@thread.skype/sharedWithTeams/ece6f0a1-5g39-498b-be79-edf6c8fc4d82')
    .version('beta')
    .delete();

```