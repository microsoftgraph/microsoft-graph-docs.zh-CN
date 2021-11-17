---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6a84a0fb32916b9d93932b807f42615b3d3ad6010b5db7b4552c898295e434c5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219662"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let members = await client.api('/directoryRoles/23f3b4b4-8a29-4420-8052-e4950273bbda/members')
    .get();

```