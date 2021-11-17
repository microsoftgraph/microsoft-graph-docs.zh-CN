---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 68671d70365e46d73c71a0176b0d61b1f04618b628bc69442ef8636cf80fef2d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277970"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let store = await client.api('/sites/microsoft.sharepoint.com,c6482504-4a85-4b21-858a-7e88dafc8232,d90ca07d-25c0-4ce7-864b-d68b607e697f/termStore')
    .version('beta')
    .get();

```