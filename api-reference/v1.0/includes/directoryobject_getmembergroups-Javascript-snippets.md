---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8d94193387befabbb8d5724b993c356c5271dae2
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34458097"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const String = {
  securityEnabledOnly: true
};

let res = await client.api('/directoryObjects/{object-id}/getMemberGroups')
    .post(String);

```