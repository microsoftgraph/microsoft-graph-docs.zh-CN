---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2dbff2fbfa7be521f83c5a5460f75cce26a8e611
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49690104"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Chats["19:ea28e88c00e94c7786b065394a61f296@thread.v2"].InstalledApps["NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg="]
    .Request()
    .DeleteAsync();

```