---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 218f60e3c618fff0a431afef8b59aaf74125db9e
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994809"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var connectionOperation = await graphClient.Connections["contosohr"].Operations["3ed1595a-4bae-43c2-acda-ef973e581323"]
    .Request()
    .GetAsync();

```