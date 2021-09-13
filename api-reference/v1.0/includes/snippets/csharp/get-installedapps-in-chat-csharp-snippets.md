---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 57e26134dbeadbfc80a9b560af87875ac3975590f9c5e020b2c84004c3484ce7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57107154"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamsAppInstallation = await graphClient.Chats["{chat-id}"].InstalledApps["{teamsAppInstallation-id}"]
    .Request()
    .GetAsync();

```