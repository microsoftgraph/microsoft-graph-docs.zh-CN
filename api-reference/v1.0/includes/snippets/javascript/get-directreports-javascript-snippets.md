---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3afe9d25621418629b7c67b7eabac6ddb18a63dcc1f2596d97978e8b635bc3c0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164026"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let directReports = await client.api('/me/directReports')
    .get();

```