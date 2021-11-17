---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9b2b5630a0aca48992e9e1abe61760209470f555e7830051a13d355d24f54209
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215872"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const contactFolder = {
  displayName: 'Family'
};

await client.api('/me/contactFolders/{id}/childFolders')
    .version('beta')
    .post(contactFolder);

```