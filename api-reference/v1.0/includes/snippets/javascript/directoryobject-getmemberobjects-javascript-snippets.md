---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7d1a5616bb3a7b82424f18122b099c93fe8abed0
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2019
ms.locfileid: "37428862"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  securityEnabledOnly: true
};

let res = await client.api('/directoryObjects/{object-id}/getMemberObjects')
    .post(string);

```