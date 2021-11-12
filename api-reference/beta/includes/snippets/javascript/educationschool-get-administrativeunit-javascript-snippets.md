---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 16b1639fa88bd854d2d1d84e45466c5190d33362067530edfe85a39371edcc73
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274012"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let administrativeUnit = await client.api('/education/schools/2961761D-8094-4183-A9F6-8E36E966C7D9/administrativeUnit')
    .version('beta')
    .get();

```