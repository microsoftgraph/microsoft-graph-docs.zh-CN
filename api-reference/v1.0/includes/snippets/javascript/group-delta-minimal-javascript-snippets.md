---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 12a217a87f05aaae7744bb6aa90e5e27d6e96736
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809108"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/groups/delta')
    .header('Prefer','return=minimal')
    .select('displayName,description,mailNickname')
    .get();

```