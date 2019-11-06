---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 547e551533235610f62b8248ce706efe3445f71a
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994545"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const externalItem = {
  @odata.type: "microsoft.graph.externalFile",
  acl: [
    {
      type: "user",
      value: "49103559-feac-4575-8b94-254814dfca72",
      accessType: "grant",
      identitySource: "Azure Active Directory"
    }
  ],
  createdDateTime: "2019-01-31T03:44:19.0354159Z",
  modifiedDateTime: "2019-01-31T03:44:19.0354159Z",
  createdBy: "Pradeep Gupta",
  lastModifiedBy: "Adele Vance",
  title: "Enterprise Search Graph Ingestion API",
  url: "file://filesrv02.corp.contoso.com/data/project/Enterprise Search.docx",
  name: "Enterprise Search.docx",
  extension: "docx",
  size: 8676776,
  content: "The quick brown fox jumps over the lazy dog."
};

let res = await client.api('/connections/contosofiles/items/myFile01')
    .version('beta')
    .put(externalItem);

```