---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6abb258a8b1bb7cd65fe007491551b148b0a695eef9dd167f1987f0b75eb1132
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104807"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let queries = await client.api('/compliance/ediscovery/cases/2eef613a-ca2d-42f4-89fe-84d5198ddedf/reviewSets/b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8/queries')
    .version('beta')
    .get();

```