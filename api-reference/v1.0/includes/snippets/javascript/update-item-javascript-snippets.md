---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b84d433ffb2dc33584b7f2950cc8ae13459090d4bb1070bd78e27440b4bbf5e1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279686"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const driveItem = {
  name: 'new-file-name.docx'
};

await client.api('/me/drive/items/{item-id}')
    .update(driveItem);

```