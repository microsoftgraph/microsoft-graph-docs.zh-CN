---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7f2518b9aa1f4d9a9df7ba3abeca2d128d7a5ca5a42a5720508651de6b9a8f04
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278712"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let conversation = await client.api('/groups/{id}/conversations/{id}')
    .get();

```