---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 32bec8a7c3c9d287716dd0bc8958da9cbebb433b
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37996439"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/profile/projects/{id}')
    .version('beta')
    .get();

```