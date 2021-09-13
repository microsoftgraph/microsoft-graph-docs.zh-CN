---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e04cf6b735735e36af26dc32c1166089fbdb73d9c4605c67e4142a85f6875ef7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163287"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/directoryObjects/{id}')
    .delete();

```