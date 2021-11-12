---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 04ef9f0901e303f2d498a6e2d521195ff711bee4ffc0f2e0c081c22b9aca50d1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163839"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let connectors = await client.api('/print/connectors')
    .get();

```