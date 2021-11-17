---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bd7a443ea4b462f31043221dd4908dafde2b4b2caa649e4874112163e0605221
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162472"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let messageRules = await client.api('/me/mailFolders/inbox/messagerules')
    .version('beta')
    .get();

```