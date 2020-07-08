---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c594c248d80b7b28bee24c49ea42f8f9ec783b88
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2020
ms.locfileid: "45080690"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Organization["settings"].ProfileCardProperties.Fax
    .Request()
    .DeleteAsync();

```