---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a713652b03f83fe6508e28c56ed7c8a2a90cbd56
ms.sourcegitcommit: 3834b7b0287ee71668c52c42d3465ca19366e678
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/01/2020
ms.locfileid: "43082161"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/contacts/delta')
    .header('Prefer','return=minimal')
    .select('displayName,jobTitle,mail')
    .get();

```