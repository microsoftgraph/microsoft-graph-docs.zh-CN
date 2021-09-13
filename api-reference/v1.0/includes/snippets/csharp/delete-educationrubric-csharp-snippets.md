---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6d89901a8fea8b87dd279087bb77beb5c513525173b68594780d9915d083f814
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106038"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Me.Rubrics["{educationRubric-id}"]
    .Request()
    .DeleteAsync();

```