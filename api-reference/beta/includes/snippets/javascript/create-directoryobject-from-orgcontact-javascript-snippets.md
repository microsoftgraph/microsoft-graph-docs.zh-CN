---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6111db12148041fa5b6e327f56cadb9205c99281
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945307"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  directoryObject: {
  }
};

let res = await client.api('/contacts/{id}/directReports')
    .version('beta')
    .post(directoryObject);

```