---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2e0312d8265b2e20dfb2c6f271bf20a422f2e238
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994782"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/profile/educationalActivities/{id}')
    .version('beta')
    .get();

```