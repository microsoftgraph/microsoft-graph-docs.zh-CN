---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ae339ad930a19b9bc7b4800e3c5bcaeba7af072b
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327517"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let organization = await client.api('/organization/84841066-274d-4ec0-a5c1-276be684bdd3')
    .get();

```