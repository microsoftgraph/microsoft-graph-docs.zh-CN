---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6932d123234c53eb8c67e41122a43138c930ed13
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59097857"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/roleManagement/directory/roleDefinitions/f189965f-f560-4c59-9101-933d4c87a91a')
    .delete();

```