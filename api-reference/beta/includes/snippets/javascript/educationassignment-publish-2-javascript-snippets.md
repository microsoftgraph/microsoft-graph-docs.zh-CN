---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 51ac7d91bbf5607653b428d82790b07790d8975facb84acb37d773d3439096fe
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164115"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/classes/11021/assignments/19002/publish')
    .version('beta')
    .post();

```