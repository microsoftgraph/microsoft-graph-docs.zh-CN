---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 410e85533b381b49ee388602354c225dea2ea40ad705acd708bf9ccc56191ac8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163614"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/teams/53c53217-fe77-4383-bc5a-ed4937a1aecd/tags/MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM3ZDg4M2Q4Yi1hMTc5LTRkZDctOTNiMy1hOGQzZGUxYTIxMmUjI3RhY29VSjN2RGk==')
    .version('beta')
    .delete();

```