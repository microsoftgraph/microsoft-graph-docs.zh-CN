---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6238833d36eca4a43d20e03d0709699e3188a6eb
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945147"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/me/user')
    .get();

```