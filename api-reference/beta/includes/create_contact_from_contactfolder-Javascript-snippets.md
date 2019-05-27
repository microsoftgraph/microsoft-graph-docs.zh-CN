---
description: 自动生成的文件。 不修改
ms.openlocfilehash: eb5e6738ef2c179f04475f4fba132515a92bcaa4
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34457106"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const contact = {
  parentFolderId: "parentFolderId-value",
  birthday: "2016-10-19T10:37:00Z",
  fileAs: "fileAs-value",
  displayName: "displayName-value",
  givenName: "givenName-value",
  initials: "initials-value"
};

let res = await client.api('/me/contactFolders/{id}/contacts')
    .version('beta')
    .post({contact : contact});

```