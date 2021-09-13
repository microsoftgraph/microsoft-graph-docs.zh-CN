---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5d066efa6a43c46924f22e74074c44c2844620d12e8b1457823ef408aa9719f7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105080"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let contactFolders = await client.api('/me/contactFolders')
    .get();

```