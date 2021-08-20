---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ff4b96380d3566e7c80567a492b9080abe4e88d10795c53dba43b15d7a3c9f9b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378591"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let users = await client.api('/users')
    .version('beta')
    .get();

```