---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f2090d5a378cec5cc26a53ac97117adab8c7973563dc6a22a8f64b2bf11e96a0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219062"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/compliance/ediscovery/cases/061b9a92-8926-4bd9-b41d-abf35edc7583')
    .version('beta')
    .delete();

```