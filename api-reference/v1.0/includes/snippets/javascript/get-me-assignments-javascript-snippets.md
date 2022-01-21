---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b97168007193914368101ffab2a2ed25116ebc2b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62111075"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let assignments = await client.api('/education/me/assignments')
    .get();

```