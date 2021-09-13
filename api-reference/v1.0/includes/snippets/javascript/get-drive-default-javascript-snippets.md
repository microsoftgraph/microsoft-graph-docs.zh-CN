---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ade1d33f579dd0f6548f574b12a50396f53cdc19fc7d7d7b4798a00f1769bae3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902329"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let drive = await client.api('/me/drive')
    .get();

```