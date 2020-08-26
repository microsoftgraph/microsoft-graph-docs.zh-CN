---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bdbf97a72835f2597d218f65a25b773aecda356e
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873938"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/insights/used')
    .orderby('LastUsed/LastAccessedDateTime desc')
    .get();

```