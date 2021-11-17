---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0b254068dfa21d911146c96af50868db8be866db7a9745e9cafb9aed22b10bdf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278479"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let scopedMembers = await client.api('/directoryRoles/roleTemplateId=fdd7a751-b60b-444a-984c-02652fe8fa1c/scopedMembers')
    .version('beta')
    .get();

```