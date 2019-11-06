---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 16b631e1ea6b47bb4d10a9542c976ae082b369ab
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "38000169"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const application = {
  displayName: "New display name"
};

let res = await client.api('/applications/{id}')
    .version('beta')
    .update(application);

```