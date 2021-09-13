---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: adac339bd0bd472656f8101b538a332a7a9807ce5b9bb8afad34011642e93007
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333805"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var children = await graphClient.Me.Drive.Special["{driveItem-id}"].Children
    .Request()
    .GetAsync();

```