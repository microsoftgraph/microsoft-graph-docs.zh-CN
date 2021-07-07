---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0124a08657202ebfa61c5207b0db244dc059ecc0
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2021
ms.locfileid: "53319493"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const noncustodialDataSource = {
    '@odata.id': 'https://canary.graph.microsoft.com/testprodbetancsdsaslist/compliance/ediscovery/cases/06d52284-ed81-49b8-904a-b863d3164731/noncustodialDataSources/39383530323537383742433232433246'
};

await client.api('/compliance/ediscovery/cases/06d52284-ed81-49b8-904a-b863d3164731/sourceCollections/12aab1671c834213a84ba219c06f4c5a/noncustodialSources/$ref')
    .version('beta')
    .post(noncustodialDataSource);

```