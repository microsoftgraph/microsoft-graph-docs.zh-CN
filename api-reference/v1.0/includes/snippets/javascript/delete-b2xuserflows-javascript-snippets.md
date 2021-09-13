---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e011b0851f228c8beae283ca30e03ad6ef4f9d527e7383aa58412de5087b69af
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332156"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identity/b2xUserFlows/B2X_1_Partner')
    .delete();

```