---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d76f9a12f9b5162e320718b1b765e344a1b394627a71d0eaafe73d0a66801e30
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274261"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let transitiveMembers = await client.api('/groups/{id}/transitiveMembers')
    .get();

```