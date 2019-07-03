---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 43fbc0d1b9fe3f1cdf69aa9053ed9b223ad12ce0
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35493301"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const contact = {
  parentFolderId: "parentFolderId-value",
  birthday: "datetime-value",
  fileAs: "fileAs-value",
  displayName: "displayName-value",
  givenName: "givenName-value",
  initials: "initials-value"
};

let res = await client.api('/me/contactFolders/{id}/contacts')
    .post({contact : contact});

```