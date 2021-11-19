---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3eed5f1a0cc17a86b24080a851c1fc7d6d2643f9
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61100127"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

mailFolderId := "mailFolder-id"
result, err := graphClient.Me().MailFoldersById(&mailFolderId).ChildFolders().Get(options)


```