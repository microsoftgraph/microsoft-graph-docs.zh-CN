---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8aeea6b1b22d77d4a36c0a257a1a17782a759aee
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35466916"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationClass = {
  description: "Health Level 1",
  classCode: "Health 501",
  displayName: "Health 1",
  externalId: "11019",
  externalName: "Health Level 1",
  externalSource: "sis",
  mailNickname: "fineartschool.net"
};

let res = await client.api('/education/classes')
    .post({educationClass : educationClass});

```