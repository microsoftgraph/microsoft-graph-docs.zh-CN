---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 831efa71113b3ba0b1ff892837ebd0351a187ce1
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37998158"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/profile/anniversaries/{id}')
    .version('beta')
    .get();

```