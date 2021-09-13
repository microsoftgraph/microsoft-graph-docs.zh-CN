---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 31c8d9ba71f77849f0600e762eb57e8697c442919c6adb4423a6759d0b56449d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104588"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let user = await client.api('/education/me/user')
    .get();

```