---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7f4bdd1b9f1448d16b0ae0787ab2868ef05b7e7b
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808944"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/appCatalogs/teamsApps?requiresReview=true')
    .post();

```