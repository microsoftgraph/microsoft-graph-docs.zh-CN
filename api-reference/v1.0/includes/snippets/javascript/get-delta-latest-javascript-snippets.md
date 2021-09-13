---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e2037306d29c411e0ffa366acc50dc5ebde31d740234bfbfcc96576109139b7f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104608"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/me/drive/root/delta?token=latest')
    .get();

```