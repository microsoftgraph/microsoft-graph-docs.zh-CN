---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 96b8efe23f69f86d2db53ad33b750d18b4ae8c14d36f6060a53018b7f189379c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163122"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const outlookCategory = {
  color: 'preset15'
};

await client.api('/me/outlook/masterCategories/bac262b7-485d-4739-b436-e31467d64fac')
    .version('beta')
    .update(outlookCategory);

```