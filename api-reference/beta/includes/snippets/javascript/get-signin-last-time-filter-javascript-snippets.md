---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 27673536d4f9b9eef1f65821fafa0e90ac1cee5f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50465277"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users')
    .version('beta')
    .filter('startswith(displayName,\'Eric\')')
    .select('displayName,signInActivity')
    .get();

```