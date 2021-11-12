---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0b8c8a0ea4a92eb4b7017897d88f7e3ad7da8fed5ade9dbe98ae49a73e3f57ab
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219718"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printOperation = await client.api('/print/operations/{id}')
    .version('beta')
    .get();

```