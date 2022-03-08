---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f43afad20c9f9a92ac1460e4d190086a03239183
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63351194"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sourceCollection = await client.api('/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/sourcecollections/1a9b4145d8f84e39bc45a7f68c5c5119')
    .version('beta')
    .expand('addToReviewSetOperation,custodianSources,lastEstimateStatisticsOperation')
    .get();

```