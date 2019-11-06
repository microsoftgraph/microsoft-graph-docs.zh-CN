---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c4462d3ce2cc418a8b97b2d5d0642f230b580efc
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997008"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/profile')
    .version('beta')
    .get();

```