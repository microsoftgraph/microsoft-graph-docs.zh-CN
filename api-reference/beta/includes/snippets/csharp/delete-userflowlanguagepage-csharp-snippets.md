---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e9fcc1b73866d786925b907578fa34a8129b8707
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844909"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Identity.B2cUserFlows["B2C_1_Customer"].Languages["en"].OverridesPages["phonefactor"].Content
    .Request()
    .DeleteAsync();

```