---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dc977bf579ee600129cff4d741fd3fe7f6e1c3a7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801826"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const contact = {
  parentFolderId: 'parentFolderId-value',
  birthday: '2016-10-19T10:37:00Z',
  fileAs: 'fileAs-value',
  displayName: 'displayName-value',
  givenName: 'givenName-value',
  initials: 'initials-value'
};

await client.api('/me/contactFolders/{id}/contacts')
    .version('beta')
    .post(contact);

```