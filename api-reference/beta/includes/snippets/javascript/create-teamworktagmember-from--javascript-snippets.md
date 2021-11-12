---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1b0f28ce1b0a20cb50c132ebc1760863a3cd035b4eea01c9a587a4b0fc2513e7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332471"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const teamworkTagMember = {
    userId: '97f62344-57dc-409c-88ad-c4af14158ff5'
};

await client.api('/teams/53c53217-fe77-4383-bc5a-ed4937a1aecd/tags/MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM3ZDg4M2Q4Yi1hMTc5LTRkZDctOTNiMy1hOGQzZGUxYTIxMmUjI3RhY29VSjN2RGk==/members')
    .version('beta')
    .post(teamworkTagMember);

```