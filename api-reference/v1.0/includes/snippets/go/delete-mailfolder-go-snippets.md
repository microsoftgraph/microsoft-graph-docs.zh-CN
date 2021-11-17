---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f420ac8df3759dbd3748cc2b013c4940439908dd
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60992975"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

mailFolderId := "mailFolder-id"
graphClient.Me().MailFoldersById(&mailFolderId).Delete(options)


```