---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b9fa986cfb6098868a94de980bd7d1b84316dde8
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35493503"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const contactFolder = {
  displayName: "displayName-value"
};

let res = await client.api('/me/contactFolders/{id}/childFolders')
    .post({contactFolder : contactFolder});

```