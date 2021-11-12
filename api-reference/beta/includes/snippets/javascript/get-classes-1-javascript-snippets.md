---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eabf4fc3db56181701396d11ec845030d3e2b07096e60b66a6ed7cf732f0d0e7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274389"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let classes = await client.api('/education/classes')
    .version('beta')
    .get();

```