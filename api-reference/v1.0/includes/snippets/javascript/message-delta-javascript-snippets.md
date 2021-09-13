---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aad3655ed72e144ff6c7cb1f1c0d98104948cc42d3d8168b004172e39da4f4f9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106720"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/me/mailFolders/{id}/messages/delta')
    .header('Prefer','odata.maxpagesize=2')
    .get();

```