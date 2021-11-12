---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b0834a79c4cc5be993b1a1630bce66bb3024a5b0c8e6a8f38a246d4508e831cd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162243"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var @string = await graphClient.Education.SynchronizationProfiles["{educationSynchronizationProfile-id}"]
    .UploadUrl()
    .Request()
    .GetAsync();

```