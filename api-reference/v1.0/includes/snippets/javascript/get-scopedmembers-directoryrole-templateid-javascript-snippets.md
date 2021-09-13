---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b02913a5b32a04cabbc4aac9b35a18e752de592a7f1d8ea78ded1366929fce9c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164037"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let scopedMembers = await client.api('/directoryRoles/roleTemplateId=fdd7a751-b60b-444a-984c-02652fe8fa1c/scopedMembers')
    .get();

```