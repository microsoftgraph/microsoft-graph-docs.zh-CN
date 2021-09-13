---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cb5bedaa9d6201ff384eed0da2785cf4ba9c791632c7b5dd6612cec7cf3c9126
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903898"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/events/{id}')
    .delete();

```