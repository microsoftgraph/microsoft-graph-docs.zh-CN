---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b3da084052de26807ae33fc08fa0fe4383cc6346d507e560732ea3105f6f8412
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162174"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const teamworkTag = {
  displayName: 'Finance'
};

await client.api('/teams/53c53217-fe77-4383-bc5a-ed4937a1aecd/tags/MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM3ZDg4M2Q4Yi1hMTc5LTRkZDctOTNiMy1hOGQzZGUxYTIxMmUjI3RhY29VSjN2RGk==')
    .version('beta')
    .update(teamworkTag);

```