---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1b2cace35d46cae1efe5cc63c6d641df84b5955443ea6cf417da2132c83b76ee
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101309"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const merge = {
  across: true
};

await client.api('/me/drive/items/{id}/workbook/names/{name}/range/merge')
    .post(merge);

```