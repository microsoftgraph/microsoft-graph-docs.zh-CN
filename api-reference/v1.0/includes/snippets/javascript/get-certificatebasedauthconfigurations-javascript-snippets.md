---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3a3025a425884de1d21981312f0de6fd4cd03bc6bfdb1812b4319094950dd900
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279385"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let certificateBasedAuthConfiguration = await client.api('/organization/{id}/certificateBasedAuthConfiguration')
    .get();

```