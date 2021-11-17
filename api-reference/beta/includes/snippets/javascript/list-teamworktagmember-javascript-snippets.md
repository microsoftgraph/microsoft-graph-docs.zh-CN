---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a98da9b4cc3f06cbeb08c8b082a988233a28f91512fce17d3cc8bf7a79057fd0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903642"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let members = await client.api('/teams/53c53217-fe77-4383-bc5a-ed4937a1aecd/tags/MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM3ZDg4M2Q4Yi1hMTc5LTRkZDctOTNiMy1hOGQzZGUxYTIxMmUjI3RhY29VSjN2RGk==/members')
    .version('beta')
    .get();

```