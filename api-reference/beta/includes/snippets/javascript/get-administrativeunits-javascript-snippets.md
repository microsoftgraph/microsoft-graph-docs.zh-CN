---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 26183b61c31fcc2f83c7c99b94588c701af6411bc0841e4a3a539c74cb6047ce
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902562"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let administrativeUnits = await client.api('/administrativeUnits')
    .version('beta')
    .get();

```