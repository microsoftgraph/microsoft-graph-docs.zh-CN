---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 318cc5cee072e7a0cb202d643d69bc10390705fb
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66502841"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const ediscoveryNoncustodialDataSource = {
    '@odata.id': 'https://graph.microsoft.com/beta/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/noncustodialDataSources/39333641443238353535383731453339'
};

await client.api('/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/searches/c61a5860-d634-4d14-aea7-d82b6f4eb7af/noncustodialSources/$ref')
    .version('beta')
    .post(ediscoveryNoncustodialDataSource);

```