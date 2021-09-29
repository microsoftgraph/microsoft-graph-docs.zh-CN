---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3511d55a28afba961aa5cd5e478c06c3b30eb6a7c6ea201446e5f323f6215e6d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106167"
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