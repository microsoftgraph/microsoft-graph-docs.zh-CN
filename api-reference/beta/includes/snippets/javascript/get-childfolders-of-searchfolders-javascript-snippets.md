---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d71ea4c5c520536b91b6d79cc57aa552ec91779e52b6c8c6dd73de1f96cf8ef8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219021"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let childFolders = await client.api('/me/mailFolders/searchfolders/childFolders')
    .version('beta')
    .get();

```