---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e73d60c10e7e6b14f31d9e0172bc89bc1616dfd3817c84b7db5f3d0da45fd822
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332799"
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
    .post(contactFolder);

```