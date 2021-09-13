---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9cc58ea37cdc7e3c9a50455b18830128e39ee2e49cab3a048f925dad43b70daf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278831"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/inferenceClassification/overrides/98f5bdef-576a-404d-a2ea-07a3cf34af4r')
    .delete();

```