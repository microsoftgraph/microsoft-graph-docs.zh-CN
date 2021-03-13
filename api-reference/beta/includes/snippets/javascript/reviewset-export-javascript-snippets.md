---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 493ba17aa41566012bb7f28730ca89da61ce59b7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772862"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const _export = {
  outputName: '2020-12-06 Contoso investigation export',
  description: 'Export for the Contoso investigation',
  exportOptions: 'originalFiles,fileInfo,tags',
  exportStructure: 'directory'
};

await client.api('/compliance/ediscovery/cases/99e865fc-e29f-479a-ba83-9e58eb017103/reviewsets/e44ac2cb-f8b4-4fd8-aa1c-1391b46ba9cc/export')
    .version('beta')
    .post(_export);

```