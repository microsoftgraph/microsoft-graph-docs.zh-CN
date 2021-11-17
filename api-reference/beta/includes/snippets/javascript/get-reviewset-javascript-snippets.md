---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 15b629c772a7d9b1bed81294cdaf2e67260df7d487566266fcda49df866f3a72
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274171"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let reviewSet = await client.api('/compliance/ediscovery/cases/6f65a8e4-c6a0-4cff-8a81-c9ab5df7290d/reviewSets/0157910c-57ce-4e48-bd4b-90f3c88ca32e')
    .version('beta')
    .get();

```