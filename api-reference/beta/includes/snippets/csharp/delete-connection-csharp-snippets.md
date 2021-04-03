---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2e9c2df713e84ae56d4fcf04a40cb61ffeb3196c
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51573177"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Connections["{externalConnectors.externalConnection-id}"]
    .Request()
    .DeleteAsync();

```