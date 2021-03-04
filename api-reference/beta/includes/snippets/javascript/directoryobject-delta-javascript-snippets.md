---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7e4dbd3f309ebcac36843d57bb45716e6ffbeb87
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436925"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directoryObjects/delta')
    .version('beta')
    .filter('isOf(\'Microsoft.Graph.User\') or isOf(\'Microsoft.Graph.Group\')')
    .get();

```