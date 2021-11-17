---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e9cca1ebbc690a1ce522b5edbe1afe0a6471d66a3560ba0c6eabf00234c3aba5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278905"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sites = await client.api('/sites/{site-id}/sites')
    .version('beta')
    .get();

```