---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 99d5f9824573c54427be387d90183b82a083bedc
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994641"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/external/connections')
    .version('beta')
    .get();

```