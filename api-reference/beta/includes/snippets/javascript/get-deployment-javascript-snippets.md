---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 06a008b12b0418c67c2c9e99e44632d2a891a6972ae131cb6fb35ffc8a2c6b7f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104648"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let deployment = await client.api('/admin/windows/updates/deployments/b5171742-1742-b517-4217-17b5421717b5')
    .version('beta')
    .get();

```