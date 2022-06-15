---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 70b1eb6902e3e1036a26c53dd3976f5947e1ba9c
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092148"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let ediscoveryNoncustodialDataSource = await client.api('/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/noncustodialdatasources/35393639323133394345384344303043')
    .version('beta')
    .expand('dataSource')
    .get();

```