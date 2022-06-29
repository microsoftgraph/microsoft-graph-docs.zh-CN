---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 961eb9bd7e3217bfa099dd6f97fccb6cc621e1fc
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66502509"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/settings/resettodefault')
    .version('beta')
    .post();

```