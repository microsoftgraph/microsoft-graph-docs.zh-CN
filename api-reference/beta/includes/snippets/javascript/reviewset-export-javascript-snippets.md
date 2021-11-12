---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e55270fde50484ba89c50a9ecf976dad38ce082d1d10693d45ec9f99cd960731
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105800"
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