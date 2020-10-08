---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aa74332b562ded029cb98cc2c16f69b2c6d035f2
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/07/2020
ms.locfileid: "48373601"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{id}/channels')
    .version('beta')
    .filter('membershipType eq 'private'')
    .get();

```