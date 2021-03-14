---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dea8c001de64e9a7a9af4767ff5038b0e6c61cec
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805726"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const contactFolder = {
  displayName: 'displayName-value'
};

await client.api('/me/contactFolders/{id}/childFolders')
    .post(contactFolder);

```