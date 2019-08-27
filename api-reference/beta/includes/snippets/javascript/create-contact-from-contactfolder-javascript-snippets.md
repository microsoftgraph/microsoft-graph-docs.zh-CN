---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 86d81fc8e9c5dfd8a15009a39ed92af61b38cf5a
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636545"
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
    .post(contact);

```