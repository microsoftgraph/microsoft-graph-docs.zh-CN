---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 70a28849083f8fd6bcacc9fdfa777859a5fcf5a3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35467679"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups')
    .filter('hasMembersWithLicenseErrors+eq+true,')
    .select('id,displayName')
    .get();

```