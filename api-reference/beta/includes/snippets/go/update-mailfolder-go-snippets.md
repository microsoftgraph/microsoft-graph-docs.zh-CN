---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6b6b7e28e27d7e50b9acfb92845fe76e166c6b91
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61020732"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

mailFolderId := "mailFolder-id"
graphClient.Me().MailFoldersById(&mailFolderId).Patch(options)


```