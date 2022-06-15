---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 678c34dfbbfb187fec89373cbf49d2b0649f2c45
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095879"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const _export = {
    outputName: 'Export reviewset query via API',
    description: 'Export for the Contoso investigation 2',
    exportOptions: 'originalFiles,fileInfo,tags',
    exportStructure: 'directory'
};

await client.api('/security/cases/eDiscoverycases/58399dff-cebe-478f-b1af-d3227f1fd645/reviewSets/273f11a1-17aa-419c-981d-ff10d33e420f/queries/fcb86cd1-50e0-427c-840e-ba6f087364e5/export')
    .version('beta')
    .post(_export);

```