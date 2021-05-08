---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: caa9a52583175a039e14607828445250cf4d5a39
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52238941"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let updatableAsset = await client.api('/admin/windows/updates/updatableAssets/5c55730b-730b-5c55-0b73-555c0b73555c')
    .version('beta')
    .get();

```