---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7cdddb4f44c7de60a1e84ef52a607bb0246ee20ec1f29518d81de384ec5abd66
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105786"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let asHierarchy = await client.api('/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/asHierarchy')
    .version('beta')
    .get();

```